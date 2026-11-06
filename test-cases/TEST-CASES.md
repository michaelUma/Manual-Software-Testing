# Manual Test Cases

Use a fresh test account and an authorized test environment. Record actual results and evidence.

| ID | Scenario | Steps | Expected result | Priority |
|---|---|---|---|---|
| TC-001 | Register with valid details | Open registration; enter valid synthetic name, email and compliant password; submit | Account is created and confirmation is shown | High |
| TC-002 | Register with invalid email | Enter malformed email and submit | Validation message appears; account is not created | High |
| TC-003 | Required registration fields | Submit registration with required fields empty | Required-field messages appear | Medium |
| TC-004 | Login with valid credentials | Enter an active test account's credentials | User reaches authenticated area | High |
| TC-005 | Login with incorrect password | Enter valid test email and incorrect password | Access is denied with a safe error | High |
| TC-006 | Logout | Sign in and select logout | Session ends; protected page requires authentication | High |
| TC-007 | Create a task | Sign in; enter a title; save | Task appears once in the task list | High |
| TC-008 | Create task with blank title | Submit task form with title empty | Validation prevents invalid task creation | Medium |
| TC-009 | Edit a task | Change an existing task title and save | Updated title persists | High |
| TC-010 | Complete a task | Mark an active task complete | Completion state is visible and persists | Medium |
| TC-011 | Search existing task | Search using a known title fragment | Matching task is displayed | Medium |
| TC-012 | Search no-match term | Search for a unique nonexistent term | Clear empty-state message appears | Low |
| TC-013 | User data isolation | Sign in as user A, create task; sign in as user B | User B cannot view or modify user A's task | Critical |
| TC-014 | Session after logout | Log out, then revisit a protected URL | User is redirected or denied access | High |

## Execution record
For each run, record: date, tester, build, environment, test ID, actual result, status, evidence reference, and linked defect ID.
