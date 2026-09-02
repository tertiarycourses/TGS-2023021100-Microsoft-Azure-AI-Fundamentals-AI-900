# Lab 05 — Language: Text Analysis, PII, and Clean Inputs

**Duration:** 60 minutes
**Alignment:** Topic 2 · K5, K7, K9, K10, K11, A3, A5
**Tools:** Microsoft Foundry; Azure AI Language tool; JSON

> Microsoft interfaces evolve. Follow the named resource, state and evidence contract. If a label differs, use the current equivalent and record the difference in the issue log.

## Objective

Analyze text, detect language and PII, clean malformed input, and verify the output contract.

## Scenario

A service desk wants useful themes from feedback while preventing personal data from entering reports.

## Deliverable

A before/after clean-data record, text-analysis output, PII-redaction evidence and schema validation.

## Before you start

- Use only the trainer-approved Azure subscription, region and resource group.
- Never paste keys, tokens, personal data or confidential documents into evidence.
- Record resource names and model versions before running tests.
- Keep this lab folder intact; save your work only under the evidence folder.

## Detailed procedure

### 1. Open samples/customer-feedback.csv and identify blank, duplicate, mixed-language and PII-bearing rows.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 2. Copy the file to evidence/customer-feedback-clean.csv and remove duplicates while preserving one auditable row identifier.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 3. Normalize whitespace and blank values; do not replace unknown facts with invented values.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 4. Use a general-purpose model to summarize the cleaned feedback into three evidence-backed themes.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 5. Use the specialized text-analysis tool to detect language for the supplied multilingual samples.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 6. Run PII detection and record category, span and redacted output without exposing the original PII in screenshots.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 7. Inspect the generated client-code example and identify endpoint, credential mechanism, request payload and response fields.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 8. Validate evidence/text-analysis.json against samples/text-analysis-schema.json.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 9. Record any NaN/unknown language, over-redaction or missed PII as an issue with severity and owner.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 10. Delete resources or the lab resource group after trainer verification.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

## Acceptance checks

- [ ] Clean dataset preserves row IDs
- [ ] Summary cites source themes
- [ ] Language and PII outputs recorded
- [ ] JSON validates against schema
- [ ] No raw PII is published

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

- MicrosoftLearning/mslearn-ai-fundamentals: 03b-text-analysis.md
- Adapted for TGS-2023021100 v10.0; current-source review date: 2 September 2026.
