# Defect Classification and Severity Summary

## Summary Counts by Category and Severity

| Category | Critical | Major | Minor | Total |
|---|:---:|:---:|:---:|:---:|
| **Ambiguity** | 1 | 0 | 0 | **1** |
| **Vagueness** | 0 | 2 | 1 | **3** |
| **Incompleteness** | 1 | 4 | 0 | **5** |
| **Contradiction** | 3 | 0 | 0 | **3** |
| **Non-Verifiability** | 0 | 1 | 0 | **1** |
| **Redundancy** | 0 | 0 | 1 | **1** |
| **Infeasibility** | 1 | 0 | 0 | **1** |
| **Untraceability** | 1 | 0 | 0 | **1** |
| **Total** | **7** | **7** | **2** | **16** |

## Key Verification Takeaways
1. **High Criticality in Safety & Invariants:** 43.8% of identified defects are **Critical**, predominantly rooted in thermal contradictions (S7 vs. S8) and custodial ownership violations (S4 vs. S5).
2. **Dominance of Incompleteness:** Incompleteness accounts for 31.3% of all issues, stemming from omitted edge cases like chamber capacity limits, non-integer quota handling, and missing inspection protocols.
