# Lab 06 — Speech, Translation, and Conversational AI

**Duration:** 60 minutes
**Alignment:** Topic 2 · K7, K8, K9, A2, A3
**Tools:** Microsoft Foundry; Azure Speech Voice Live or Speech; Translator design worksheet

> Microsoft interfaces evolve. Follow the named resource, state and evidence contract. If a label differs, use the current equivalent and record the difference in the issue log.

## Objective

Use speech input/output, design a translation contract, and define a human handoff for conversational AI.

## Scenario

A multilingual support team needs a voice interaction that fails safely in noisy conditions.

## Deliverable

A transcript/output evidence pack, translation message contract and escalation decision table.

## Before you start

- Use only the trainer-approved Azure subscription, region and resource group.
- Never paste keys, tokens, personal data or confidential documents into evidence.
- Record resource names and model versions before running tests.
- Keep this lab folder intact; save your work only under the evidence folder.

## Detailed procedure

### 1. Create or open the Foundry project and select a trainer-approved speech-capable agent or Speech resource.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 2. Configure a neutral system instruction that states the support scope and prohibited actions.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 3. Connect the Speech Voice Live experience or trainer-approved Speech interface.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 4. Read samples/support-utterances.txt in a quiet setting and record transcription evidence.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 5. Repeat one utterance with background noise or a deliberate accent variation and compare the transcript.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 6. Generate speech from the approved response and note voice, language and output format.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 7. Complete samples/translation-contract.json with source language, target language, content and correlation ID.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 8. Design a handoff rule using confidence/uncertainty, harmful-content flag and repeated-failure count.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 9. Record consent, retention and accessibility controls in evidence/conversation-controls.md.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 10. Remove recordings containing personal data and clean up billable resources.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

## Acceptance checks

- [ ] Speech input and output both evidenced
- [ ] Noise/accent difference discussed
- [ ] Translation contract is valid JSON
- [ ] Handoff rule is testable
- [ ] Consent and retention addressed

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

- MicrosoftLearning/mslearn-ai-fundamentals: 04a-speech.md; legacy v9 slides 171-200
- Adapted for TGS-2023021100 v10.0; current-source review date: 2 September 2026.
