# Lab 07 evidence checklist

Learner:
Date:
Resource group / project:
Model or service version:

- [ ] Checkpoint 1: Open the Content Understanding or information-extraction playground in the Foundry project.
- [ ] Checkpoint 2: Run the Read analyzer on samples/receipt.png and capture raw OCR evidence.
- [ ] Checkpoint 3: Run the receipt or layout analyzer and compare structured fields with the visible document.
- [ ] Checkpoint 4: Record merchant, date, currency, subtotal, tax and total with confidence or uncertainty notes.
- [ ] Checkpoint 5: Transform the result into evidence/receipt-normalized.json using the supplied canonical field names and ISO date/currency conventions.
- [ ] Checkpoint 6: Validate the normalized document against samples/receipt-schema.json and correct type/required-field failures.
- [ ] Checkpoint 7: Design an Azure AI Search index with key, searchable, filterable, sortable and facetable attributes.
- [ ] Checkpoint 8: Map the normalized document fields into the index and identify which fields must not be searchable.
- [ ] Checkpoint 9: Define a human-review queue for missing totals, low confidence and arithmetic mismatch.
- [ ] Checkpoint 10: Document RBAC, data retention, lineage and cleanup controls.

## Validation
- [ ] Raw and structured outputs compared
- [ ] Normalized JSON validates
- [ ] Index attributes are justified
- [ ] Low-quality records route to review
- [ ] Lineage and access controls documented

Cleanup timestamp:
Trainer verification:
