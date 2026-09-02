# Lab 09 — Anomaly Evidence, Content Safety, Security, and Governance

**Duration:** 60 minutes
**Alignment:** Topic 3 · K6, K7, K8, A3
**Tools:** Spreadsheet or Python; Microsoft Foundry safety guardrails; Azure governance worksheet

> Microsoft interfaces evolve. Follow the named resource, state and evidence contract. If a label differs, use the current equivalent and record the difference in the issue log.

## Objective

Compute anomaly evidence, test content-safety categories, and produce an actionable issue/governance report.

## Scenario

Operations must replace a retired managed anomaly service without losing detection evidence or escalation controls.

## Deliverable

A reproducible anomaly table, safety-severity results, issue report, access model and cost/cleanup checklist.

## Before you start

- Use only the trainer-approved Azure subscription, region and resource group.
- Never paste keys, tokens, personal data or confidential documents into evidence.
- Record resource names and model versions before running tests.
- Keep this lab folder intact; save your work only under the evidence folder.

## Detailed procedure

### 1. Open samples/timeseries.csv and calculate the rolling mean and residual columns using the supplied formula notes.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 2. Apply the stated threshold rule and mark each point normal or anomalous; do not tune the threshold after seeing the answer.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 3. Chart observed value, baseline and alert threshold; annotate the first true alert and one false-positive risk.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 4. Document why Azure AI Anomaly Detector retirement requires a migration plan rather than continued provisioning instructions.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 5. Open the Foundry safety/guardrails experience or the trainer-approved Content Safety interface.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 6. Run the supplied safe, borderline and unsafe samples; record category and severity without adding harmful detail.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 7. Compare the service output with the organisation's escalation threshold and record disagreements.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 8. Complete evidence/issue-report.md with reproduction, expected/actual results, evidence, impact, owner and remediation.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 9. Add RBAC, key protection, logging, budget and human-review controls to evidence/governance-checklist.md.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 10. Clean up resources and retain only redacted evidence.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

## Acceptance checks

- [ ] Anomaly rule is reproducible
- [ ] Retirement/migration risk stated
- [ ] Safety categories and severities recorded
- [ ] Issue report has owner and remediation
- [ ] Security, cost and cleanup controls complete

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

- Legacy v9 slides 206-213; Microsoft updated exercise replacing Anomaly Detector with Content Safety
- Adapted for TGS-2023021100 v10.0; current-source review date: 2 September 2026.
