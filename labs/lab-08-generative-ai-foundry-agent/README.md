# Lab 08 — Generative AI and Agents in Microsoft Foundry

**Duration:** 65 minutes
**Alignment:** Topic 1 · K1, K6, K7, K8, A1, A2, A3
**Tools:** Microsoft Foundry; model catalog; chat playground; agent playground

> Microsoft interfaces evolve. Follow the named resource, state and evidence contract. If a label differs, use the current equivalent and record the difference in the issue log.

## Objective

Deploy a model, configure instructions and grounding, evaluate responses, and record safety controls.

## Scenario

A policy assistant must answer only from approved material and escalate when evidence is absent.

## Deliverable

A model deployment and agent configuration with grounded tests, refusal evidence and model-card controls.

## Before you start

- Use only the trainer-approved Azure subscription, region and resource group.
- Never paste keys, tokens, personal data or confidential documents into evidence.
- Record resource names and model versions before running tests.
- Keep this lab folder intact; save your work only under the evidence folder.

## Detailed procedure

### 1. Create or open a Foundry project and inspect model catalog availability for the trainer-approved region.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 2. Deploy a small trainer-approved chat model; record deployment name, model version and quota/cost note.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 3. Run the baseline prompt in samples/prompt-tests.csv and capture the response.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 4. Add system instructions that constrain scope, require source attribution and specify an uncertainty response.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 5. Attach the supplied policy document or trainer-approved knowledge source for grounding.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 6. Save the configuration as an agent if the service is available; otherwise preserve the playground configuration evidence.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 7. Run grounded, out-of-scope, ambiguous and unsafe test cases from samples/prompt-tests.csv.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 8. Score groundedness, relevance, completeness and safety in evidence/evaluation.csv.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 9. Inspect the generated client-code example and identify endpoint, authentication and message payload fields.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 10. Complete evidence/model-card.md and delete the deployment/resource group when instructed.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

## Acceptance checks

- [ ] Model version and deployment recorded
- [ ] Instructions constrain scope
- [ ] Grounded and refusal tests captured
- [ ] Evaluation uses explicit criteria
- [ ] Cost and cleanup documented

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

- MicrosoftLearning/mslearn-ai-fundamentals: 02a-generative-ai.md
- Adapted for TGS-2023021100 v10.0; current-source review date: 2 September 2026.
