# Agent Stock Eyes

**Agent Stock Eyes** is an intelligent, evidence-led stock-auditing platform that reconciles purchases, receipts, supplier invoices, sales, physical inventory, documented leakage, and other stock movements to identify variances and generate traceable audit reports.

## The problem

Stock audits are often conducted across spreadsheets, disconnected documents, physical count sheets, and verbal explanations. This makes it difficult to determine:

* What was ordered, received, invoiced, sold, or consumed.
* What stock should remain at a specific cutoff time.
* Whether apparent shortages are explained by physical stock, leakage, authorized consumption, or other movements.
* Which inconsistencies require investigation.
* How to turn audit work into a quantified, evidence-supported report.

Agent Stock Eyes is intended to guide this entire process in one auditable workspace.

## Core audit journey

The system follows stock from its source to its final outcome:

1. Purchase order.
2. Goods receipt and acceptance.
3. Supplier invoice.
4. Storage and departmental transfers.
5. Production, conversion, or portioning.
6. Sale or authorized consumption.
7. Physical stock count.
8. Documented wastage, damage, or spoilage.
9. Unresolved shortages or unexplained overages.
10. Investigation, evidence capture, findings, and reporting.

## Planned capabilities

* Business item and unit-of-measure master data.
* Mother-item, child-item, recipe, portion, and yield relationships.
* CSV and spreadsheet ingestion.
* Intelligent item and field-mapping suggestions.
* Deterministic unit conversion and stock reconciliation.
* Purchase-order, receipt, and invoice matching.
* Sales-versus-stock analysis.
* Physical stock reconciliation by location and department.
* Documented leakage and authorized non-sales movement analysis.
* COGS, gross-margin, conversion-rate, and financial-impact calculations.
* Prioritized anomalies and control exceptions.
* Item-level investigation workspaces.
* Management explanations and supporting evidence.
* Traceable, reproducible, and versioned audit reports.

## Core principles

Agent Stock Eyes must be:

* **Evidence-led:** Every important conclusion should be supported by source records or reviewed evidence.
* **Deterministic:** Authoritative quantities, costs, conversions, and financial metrics must be calculated by testable code.
* **Traceable:** Figures should be traceable to their original files, records, mappings, and formulas.
* **Fraud-safe:** An unexplained variance must not automatically be described as theft or fraud.
* **Human-reviewed:** AI may assist with extraction, mapping, investigation, and drafting, but it must not invent or approve evidence.
* **Configurable:** Thresholds, units, item relationships, and business policies should not be silently hard-coded.
* **Auditable:** Corrections, overrides, approvals, explanations, and report changes must retain a history.

## Important distinctions

The system must keep the following outcomes separate:

* Stock physically on hand.
* Documented wastage, damage, or spoilage.
* Authorized non-sales consumption.
* Supplier returns and verified adjustments.
* Documented shortages.
* Recovered or charged shortages.
* Unresolved shortages.
* Unexplained overages.
* Data-quality and cutoff limitations.

Stock that has not yet been sold is not automatically missing. Potential revenue associated with unexplained stock is revenue at risk, not proven lost sales.

## Current status

This repository is in its initial product-definition and development stage.

The first development milestone will establish a working vertical slice covering:

* Business and item master data.
* Audit-case creation.
* Structured record ingestion.
* Item and unit mapping.
* A canonical stock-movement ledger.
* Deterministic reconciliation.
* Investigation and evidence capture.
* Reproducible audit-report generation.

## Product specification

The comprehensive product and development specification will be maintained at:

`docs/agent-stock-eyes-master-context.md`

Development agents should read the complete specification before implementing business logic. They should begin with repository discovery and gap analysis, preserve existing work, document assumptions, and build the smallest testable end-to-end vertical slice.

## Product direction

Agent Stock Eyes is being developed as an operational auditing system—not merely an inventory dashboard and not an autonomous fraud detector.

Its authority must come from verified records, transparent mappings, deterministic calculations, explicit business rules, preserved provenance, human-reviewed evidence, and reproducible reports.
