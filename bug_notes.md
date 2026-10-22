# Bug Notes & Audit Trail

| Bug | Evidence / Failed Test | Cause | Fix |
| :--- | :--- | :--- | :--- |
| **Average Calculation** | Returned `135.0` instead of `90.0` for `[80, 90, 100]`; caused `ZeroDivisionError` for single-mark input `[40]`[cite: 5]. | Code divided by `len(marks) - 1` instead of total count[cite: 5]. | Changed denominator to `len(marks)`[cite: 5]. |
| **Passing Boundary** | A mark of `40` returned `False` (treated as failing)[cite: 5]. | Used strict greater-than comparison (`>`) instead of inclusive (`>=`)[cite: 5]. | Updated condition to use `>= PASS_MARK`[cite: 5]. |
| **Grade Ordering** | A score of `95` returned `"First"` instead of `"Distinction"`[cite: 5]. | The `>= 60` condition was evaluated before `>= 90`[cite: 5]. | Reordered condition checks to evaluate `>= 90` first[cite: 5]. |
