# Lab 03 — Azure Machine Learning AutoML and Model Lifecycle

**Duration:** 70 minutes
**Alignment:** Topic 1 · K3, K4, K6, A1, A2
**Tools:** Azure Machine Learning studio; Automated ML; CSV data asset

> Microsoft interfaces evolve. Follow the named resource, state and evidence contract. If a label differs, use the current equivalent and record the difference in the issue log.

## Objective

Configure an AutoML regression experiment, interpret ranking evidence, and document deployment controls.

## Scenario

Contoso Mobility needs a repeatable demand-forecast experiment that its service provider can review.

## Deliverable

An AutoML experiment record with data, task, target, compute, metric, best-model evidence and deployment decision.

## Before you start

- Use only the trainer-approved Azure subscription, region and resource group.
- Never paste keys, tokens, personal data or confidential documents into evidence.
- Record resource names and model versions before running tests.
- Keep this lab folder intact; save your work only under the evidence folder.

## Detailed procedure

### 1. Create or open an Azure Machine Learning workspace in the trainer-approved subscription and region.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 2. Create a tabular data asset from samples/daily-bike-share.csv and preview the schema.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 3. Confirm rentals is the numeric target and exclude date-derived identifiers that could leak the answer.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 4. Start an Automated ML regression job, select serverless or trainer-approved compute, and set a conservative timeout.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 5. Choose normalized root mean squared error or another trainer-approved primary metric and record the choice.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 6. Submit the job and capture the job status, experiment name and data asset version.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 7. When complete, inspect the model leaderboard, validation metric and residual or predicted-versus-true chart.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 8. Open the best model and record algorithm, transformations and feature-importance evidence where available.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 9. Complete evidence/model-card.md with intended use, limitations, metric threshold, owner and monitoring trigger.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 10. Do not deploy unless instructed; document the endpoint authentication and monitoring controls that would be required.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 11. Delete compute or the resource group after evidence review to avoid unnecessary cost.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

## Acceptance checks

- [ ] Versioned data asset recorded
- [ ] Regression target and metric justified
- [ ] Best model evidence captured
- [ ] Model card includes limitations
- [ ] Cleanup confirmed

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

- MicrosoftLearning/AI-900-AIFundamentals: 02-module-02.md; legacy v9 slides 59-92
- Adapted for TGS-2023021100 v10.0; current-source review date: 2 September 2026.
