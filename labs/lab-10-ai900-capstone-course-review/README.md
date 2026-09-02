# Lab 10 — AI-900 Capstone: End-to-End Azure AI Solution Review

**Duration:** 80 minutes
**Alignment:** Topic 4 · K1-K11, A1-A5
**Tools:** Architecture worksheet; prior lab evidence; Microsoft Foundry; Azure AI Search design

> Microsoft interfaces evolve. Follow the named resource, state and evidence contract. If a label differs, use the current equivalent and record the difference in the issue log.

## Objective

Integrate service selection, workflow deployment, issue reporting, interoperability, cleaning and governance into one evidence-backed design.

## Scenario

Contoso must approve one cross-service Azure AI solution for product feedback, receipts and policy support.

## Deliverable

A final architecture, data contract, evidence matrix, issue register, validation plan and resource-cleanup record.

## Before you start

- Use only the trainer-approved Azure subscription, region and resource group.
- Never paste keys, tokens, personal data or confidential documents into evidence.
- Record resource names and model versions before running tests.
- Keep this lab folder intact; save your work only under the evidence folder.

## Detailed procedure

### 1. Choose one supplied capstone scenario and list its users, inputs, required outputs, data classification and success measures.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 2. Select Azure services for ingestion, AI processing, knowledge retrieval and user interaction; justify each boundary.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 3. Draw the end-to-end flow using the supplied architecture template and label every persisted data store.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 4. Define the canonical JSON data contract and map source fields to target fields.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 5. Apply the cleaning rules for missing, duplicate, malformed and sensitive data.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 6. Link at least one evidence item from Labs 1-9 to every major component.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 7. Add a human-review decision point for low confidence, harmful content, anomaly or missing grounding.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 8. Complete the issue register with severity, owner, workaround and acceptance decision.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 9. Complete the security, privacy, responsible-AI, monitoring and cost controls.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 10. Run a peer review against evidence/capstone-checklist.md and resolve all critical gaps.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 11. Submit the evidence pack to the trainer-approved LMS location and clean up all temporary Azure resources.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

## Acceptance checks

- [ ] Architecture names inputs, outputs and stores
- [ ] Canonical schema and cleaning rules included
- [ ] Each component has evidence
- [ ] Human review and issue ownership are explicit
- [ ] Cleanup is confirmed

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

- TertiaryCourses legacy Lab 10, updated as a skills-based capstone
- Adapted for TGS-2023021100 v10.0; current-source review date: 2 September 2026.
