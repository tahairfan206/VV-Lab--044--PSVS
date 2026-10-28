# PSVS Requirement Defect Taxonomy

This document establishes the 8 standard verification defect classifications applied during formal requirements inspections.

## 1. Ambiguity
- **Definition:** A statement that allows two or more distinct, valid interpretations without a defined decision rule.
- **Example:** *"The system shall accept seed boxes only from registered depositors"* does not clarify whether registration status must be verified per transaction or if cached session data suffices.

## 2. Vagueness
- **Definition:** A statement using subjective or unquantified modifiers lacking concrete boundaries.
- **Example:** *"Each chamber can hold a large number of boxes"* relies on the subjective term "large number" rather than an integer ceiling.

## 3. Incompleteness
- **Definition:** Omission of necessary operational modes, edge conditions, exception handling, or boundary values.
- **Example:** Mandating a 20% annual quota without defining integer rounding rules for small inventories (e.g., 20% of 3 boxes).

## 4. Contradiction
- **Definition:** Two or more statements that impose mutually exclusive constraints or states that cannot simultaneously hold true.
- **Example:** Requiring that chamber temperature *never* rise above -18°C while simultaneously allowing it to warm to 0°C for maintenance.

## 5. Non-Verifiability
- **Definition:** A requirement that cannot be verified or disproven by any deterministic test, inspection, or mathematical proof.
- **Example:** *"The system shall keep a good audit trail of all actions"* cannot be validated because "good" is not an objective, measurable metric.

## 6. Redundancy
- **Definition:** Duplicate, superfluous, or overlapping statements where one requirement is completely subsumed by another.
- **Example:** Stating chambers hold a "large number" of boxes while another statement specifies exact numerical capacities for all chambers.

## 7. Infeasibility
- **Definition:** A requirement that violates physical laws, system boundary constraints, or fundamental domain principles.
- **Example:** Requiring non-destructive monitoring of biological viability inside tamper-evident sealed boxes without opening them.

## 8. Untraceability
- **Definition:** References to undefined external roles, protocols, or entities lacking formal identifiers or source mapping.
- **Example:** Allowing emergency release to *"any requesting party"* without specifying the registry, authority matrix, or legal basis.
