# Lab 04 — Computer Vision, Image Analysis, and OCR

**Duration:** 65 minutes
**Alignment:** Topic 2 · K3, K7, K8, A2, A3
**Tools:** Microsoft Foundry; vision-capable model; Content Understanding OCR

> Microsoft interfaces evolve. Follow the named resource, state and evidence contract. If a label differs, use the current equivalent and record the difference in the issue log.

## Objective

Analyze an image, compare vision outputs with source evidence, and report accuracy or privacy issues.

## Scenario

A product-quality team needs visual inspection and text extraction without treating model output as ground truth.

## Deliverable

An image-analysis result, OCR extraction, confidence review and issue report.

## Before you start

- Use only the trainer-approved Azure subscription, region and resource group.
- Never paste keys, tokens, personal data or confidential documents into evidence.
- Record resource names and model versions before running tests.
- Keep this lab folder intact; save your work only under the evidence folder.

## Detailed procedure

### 1. Open a Foundry project and deploy or select a trainer-approved vision-capable model.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 2. Upload samples/store-shelf.jpg and ask for objects, scene description and any visible text.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 3. Record the prompt, model/deployment name and response in evidence/vision-results.md.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 4. Compare each detected object with the image; mark true positive, false positive or missed object.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 5. Open the Content Understanding or information-extraction playground and select the Read/OCR analyzer.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 6. Upload samples/receipt.png and run analysis.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 7. Compare extracted text and bounding regions with the image; record at least two correct and one uncertain item.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 8. State the confidence or business rule that triggers human review when confidence is unavailable or low.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 9. Complete evidence/issue-log.md with reproduction steps, expected result, actual result, impact and owner.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

### 10. Redact personal information from evidence and clean up billable resources.

**Evidence checkpoint:** Update evidence/checklist.md for this checkpoint; capture a redacted screenshot or output only when it proves the named state.

## Acceptance checks

- [ ] Image input and model recorded
- [ ] Output compared with source image
- [ ] OCR uncertainty identified
- [ ] Issue report is reproducible
- [ ] Privacy and cleanup controls applied

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

- MicrosoftLearning/mslearn-ai-fundamentals: 05a-image-analysis.md and 06a-content-understanding.md
- Adapted for TGS-2023021100 v10.0; current-source review date: 2 September 2026.
