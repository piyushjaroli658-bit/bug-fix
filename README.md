# bug-fix
# Session 8: Fixing a Buggy Python Script Using AI (RED -> FIX -> GREEN Cycle)

## Overview
This repository contains the practical files for debugging Python code using unit tests and AI guidance following the **RED -> FIX -> GREEN** development cycle.

## File Contents
* **`student_utils.py`**: The corrected utility script containing functions for calculating averages, checking passing status, and assigning grades.
* **`test_student_utils.py`**: The unittest test suite containing 9 test cases verifying expected behaviors.
* **`bug_notes.md`**: Detailed documentation of bugs encountered, root causes, and fixes applied.

## How to Run Tests
Execute the test suite using Python:
\`\`\`bash
python test_student_utils.py
\`\`\`

## Test Summary
* **Number of Tests:** 9[cite: 5]
* **Final Result:** All tests passing successfully (OK)[cite: 5]

## The RED -> FIX -> GREEN Cycle
1. **RED:** Write/run tests against buggy code to prove and capture failures[cite: 5].
2. **FIX:** Modify implementation details in the source code without weakening test criteria[cite: 5].
3. **GREEN:** Rerun the unmodified test suite to verify that all tests pass[cite: 5].
