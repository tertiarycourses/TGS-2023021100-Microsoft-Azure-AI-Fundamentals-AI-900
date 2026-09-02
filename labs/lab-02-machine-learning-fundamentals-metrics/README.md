# Lab 02 — Machine Learning Fundamentals and Metrics

**Duration:** 55 minutes
**Alignment:** Topic 1 · K2, K3, K4
**Tools:** Spreadsheet or Python; samples/model-results.csv

> Microsoft interfaces evolve. Follow the named resource, state and evidence contract. If a label differs, use the current equivalent and record the difference in the issue log.

## Objective

Differentiate regression, classification and clustering and compute evidence-based model metrics.

## Scenario

A bike-share team must choose the correct technique and reject a misleading model before deployment.

## Deliverable

A technique-selection table and verified MAE, RMSE, precision, recall and confusion-matrix calculations.

## Before you start

- Use only the trainer-approved Azure subscription, region and resource group.
- Never paste keys, tokens, personal data or confidential documents into evidence.
- Record resource names and model versions before running tests.
- Keep this lab folder intact; save your work only under the evidence folder.

## Detailed procedure

### 1. Open samples/scenarios.csv and label each case regression, classification or clustering; justify the predicted output type.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 2. Identify features and label for the demand-forecasting and churn examples; flag any field that leaks the answer.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 3. Split the sample rows into training and validation partitions using the supplied split column.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 4. Use samples/model-results.csv to calculate absolute error for every regression row.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 5. Calculate MAE and RMSE; explain why RMSE increases the influence of large errors.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 6. Build a 2x2 confusion matrix from actual_class and predicted_class.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 7. Calculate precision and recall for the positive class and compare them with accuracy.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 8. Inspect the clustering sample and explain why it has no label during training.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 9. Document one data-quality defect, its likely metric impact, and a correction.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 10. Save completed calculations and the technique-selection table under evidence/.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

## Acceptance checks

- [ ] Every scenario has a justified technique
- [ ] MAE and RMSE are reproducible
- [ ] Confusion matrix totals match source rows
- [ ] Precision and recall show working
- [ ] Leakage risk documented

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

- Legacy v9 slides 57-58 and 73-119; Microsoft AI-900 study guide
- Adapted for TGS-2023021100 v10.0; current-source review date: 2 September 2026.
