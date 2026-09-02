# Lab 01 — AI Workloads, Responsible AI, and Microsoft Foundry

**Duration:** 55 minutes
**Alignment:** Topic 1 · K1, K6, K7, A1
**Tools:** Microsoft Foundry portal; Azure portal; worksheet

> Microsoft interfaces evolve. Follow the named resource, state and evidence contract. If a label differs, use the current equivalent and record the difference in the issue log.

## Objective

Classify AI workloads, map them to Azure services, inspect a Foundry project, and record responsible-AI controls.

## Scenario

Contoso Retail needs a defensible service map before its implementation partner provisions any resource.

## Deliverable

A workload-to-service decision map, responsible-AI control register, and Foundry project evidence pack.

## Before you start

- Use only the trainer-approved Azure subscription, region and resource group.
- Never paste keys, tokens, personal data or confidential documents into evidence.
- Record resource names and model versions before running tests.
- Keep this lab folder intact; save your work only under the evidence folder.

## Detailed procedure

### 1. Open the Microsoft Foundry portal and sign in with the Azure account provided for training.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 2. Create or select a resource group dedicated to the class; record subscription, region, resource-group name and owner.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 3. Create a Foundry project with a unique name and capture the project overview showing project and parent resource.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 4. Inspect the project endpoint and connected resources; redact keys or tokens from all screenshots.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 5. Classify the six scenario cards in samples/workloads.csv by input, desired output, AI workload and suitable Azure service.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 6. For each mapping, name the human decision owner and the evidence that would prove the output is acceptable.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 7. Complete evidence/responsible-ai-checklist.md for fairness, reliability and safety, privacy and security, inclusiveness, transparency and accountability.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 8. Record one limitation or uncertainty in evidence/issue-log.md and assign severity, owner and next action.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 9. Validate that no secret appears in the evidence pack and that every workload has a service and control.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 10. If you created billable resources, delete the lab resource group after the trainer verifies your evidence.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

## Acceptance checks

- [ ] Six workload rows classified
- [ ] Six responsible-AI principles addressed
- [ ] Project/resource boundary visible
- [ ] No secret values captured
- [ ] One issue assigned to an owner

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

- MicrosoftLearning/mslearn-ai-fundamentals: 00-explore-foundry.md
- Adapted for TGS-2023021100 v10.0; current-source review date: 2 September 2026.
