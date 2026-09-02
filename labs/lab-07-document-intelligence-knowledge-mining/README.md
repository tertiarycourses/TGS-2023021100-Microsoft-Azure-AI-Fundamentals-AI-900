# Lab 07 — Document Intelligence and Knowledge Mining

**Duration:** 70 minutes
**Alignment:** Topic 4 · K5, K8, K9, K10, K11, A4, A5
**Tools:** Microsoft Foundry Content Understanding; Azure AI Search design worksheet; JSON Schema

> Microsoft interfaces evolve. Follow the named resource, state and evidence contract. If a label differs, use the current equivalent and record the difference in the issue log.

## Objective

Extract document fields, normalize them to a data contract, and prepare searchable knowledge records.

## Scenario

Accounts payable needs receipt data that can move safely from extraction into search and reporting systems.

## Deliverable

A receipt extraction, cleaned interoperable JSON document, field-quality report and search-index design.

## Before you start

- Use only the trainer-approved Azure subscription, region and resource group.
- Never paste keys, tokens, personal data or confidential documents into evidence.
- Record resource names and model versions before running tests.
- Keep this lab folder intact; save your work only under the evidence folder.

## Detailed procedure

### 1. Open the Content Understanding or information-extraction playground in the Foundry project.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 2. Run the Read analyzer on samples/receipt.png and capture raw OCR evidence.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 3. Run the receipt or layout analyzer and compare structured fields with the visible document.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 4. Record merchant, date, currency, subtotal, tax and total with confidence or uncertainty notes.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 5. Transform the result into evidence/receipt-normalized.json using the supplied canonical field names and ISO date/currency conventions.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 6. Validate the normalized document against samples/receipt-schema.json and correct type/required-field failures.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 7. Design an Azure AI Search index with key, searchable, filterable, sortable and facetable attributes.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 8. Map the normalized document fields into the index and identify which fields must not be searchable.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 9. Define a human-review queue for missing totals, low confidence and arithmetic mismatch.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 10. Document RBAC, data retention, lineage and cleanup controls.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

## Acceptance checks

- [ ] Raw and structured outputs compared
- [ ] Normalized JSON validates
- [ ] Index attributes are justified
- [ ] Low-quality records route to review
- [ ] Lineage and access controls documented

## Troubleshooting

| Symptom | Likely cause | Recovery |
|---|---|---|
| Portal control or label differs | Microsoft Foundry is under continuous development | Search within the current project for the named resource or capability; record the UI difference. |
| Deployment or resource option unavailable | Region, quota, role or subscription restriction | Use a trainer-approved region/resource; do not bypass organisational policy. |
| Request fails with 401/403 | Missing role assignment or invalid credential | Verify Entra identity, RBAC and endpoint scope; never expose the key. |
| Output quality is weak | Ambiguous input, unsupported language/image, or model limitation | Preserve the failing input, tighten the test contract and route to human review. |
| Unexpected cost | Compute, deployment or resource left running | Stop or delete it and confirm in Azure Cost Management. |

## Cleanup

1. Export only the redacted evidence required by the trainer.
2. Delete the lab deployment, compute, index, project or resource group when instructed.
3. Confirm the Azure portal no longer shows a running billable resource.
4. Record the cleanup timestamp in evidence/checklist.md.

## Source lineage

- MicrosoftLearning/mslearn-ai-fundamentals: 06a-content-understanding.md and 07-foundry-iq.md
- Adapted for TGS-2023021100 v10.0; current-source review date: 2 September 2026.
