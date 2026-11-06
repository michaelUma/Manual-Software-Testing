# Manual Software Testing Portfolio

A practical QA portfolio showing how requirements become test scenarios, test cases, defect reports, execution evidence, and release recommendations.

## Application under test
A fictional task-management web app: registration, login, task creation/editing/completion/deletion, search, and logout. Use only an authorized test environment and synthetic data.

## Skills demonstrated
- Test planning, scope and risk analysis
- Functional, smoke, regression, exploratory and usability testing
- Positive, negative and boundary-value test design
- Equivalence partitioning and state-transition thinking
- Defect reporting with severity, priority and reproducible steps
- Test execution reporting and traceability

## Repository structure
- `docs/TEST-PLAN.md` — scope, risks, entry/exit criteria
- `test-cases/TEST-CASES.md` — manual test matrix
- `bug-reports/BUG-REPORT-TEMPLATE.md` — defect template and illustrative example
- `test-data/sample-test-data.csv` — synthetic test data
- `reports/TEST-EXECUTION-REPORT-TEMPLATE.md` — execution summary

## How to use
1. Review the test plan and confirm the authorized target/build.
2. Prepare synthetic accounts and test data.
3. Execute each test case and record actual results.
4. Mark each case Pass, Fail, Blocked, Not Run, or Not Applicable.
5. Log defects with evidence and link them to test case IDs.
6. Retest fixes and run relevant regression tests.
7. Complete the execution report using observed results only.

## Test case sample
| ID | Scenario | Expected result |
|---|---|---|
| MAN-001 | Register with valid details | Account created and confirmation shown |
| MAN-002 | Submit malformed email | Validation error; account not created |
| MAN-003 | Login with valid credentials | Authenticated dashboard appears |
| MAN-004 | Login with wrong password | Access denied with safe error |
| MAN-005 | Create a task | Exactly one task appears |
| MAN-006 | Submit task with blank title | Validation prevents creation |
| MAN-007 | Search for existing task | Matching task is returned |
| MAN-008 | User B requests User A's task | Access denied; no data leakage |

## Important evidence note
This repository contains templates and sample scenarios. Do not claim that tests passed or defects were observed until you execute them and attach dated, sanitized evidence.

## Author
Michael Uma — Software QA / Manual Testing Portfolio.
