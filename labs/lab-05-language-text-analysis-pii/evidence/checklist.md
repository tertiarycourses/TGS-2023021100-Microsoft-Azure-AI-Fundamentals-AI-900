# Lab 05 evidence checklist

Learner:
Date:
Resource group / project:
Model or service version:

- [ ] Checkpoint 1: Open samples/customer-feedback.csv and identify blank, duplicate, mixed-language and PII-bearing rows.
- [ ] Checkpoint 2: Copy the file to evidence/customer-feedback-clean.csv and remove duplicates while preserving one auditable row identifier.
- [ ] Checkpoint 3: Normalize whitespace and blank values; do not replace unknown facts with invented values.
- [ ] Checkpoint 4: Use a general-purpose model to summarize the cleaned feedback into three evidence-backed themes.
- [ ] Checkpoint 5: Use the specialized text-analysis tool to detect language for the supplied multilingual samples.
- [ ] Checkpoint 6: Run PII detection and record category, span and redacted output without exposing the original PII in screenshots.
- [ ] Checkpoint 7: Inspect the generated client-code example and identify endpoint, credential mechanism, request payload and response fields.
- [ ] Checkpoint 8: Validate evidence/text-analysis.json against samples/text-analysis-schema.json.
- [ ] Checkpoint 9: Record any NaN/unknown language, over-redaction or missed PII as an issue with severity and owner.
- [ ] Checkpoint 10: Delete resources or the lab resource group after trainer verification.

## Validation
- [ ] Clean dataset preserves row IDs
- [ ] Summary cites source themes
- [ ] Language and PII outputs recorded
- [ ] JSON validates against schema
- [ ] No raw PII is published

Cleanup timestamp:
Trainer verification:
