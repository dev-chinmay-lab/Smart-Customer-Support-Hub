# Test Plan — Initial Scenarios

**Status:** Test design only. Results are not yet recorded.

## Test execution template
For each test, record: Test ID, date, tester, org/environment, test data, steps, expected result, actual result, Pass/Fail, evidence link, and defect/notes.

| Test ID | Scenario | Expected result | Status |
|---|---|---|---|
| TC-001 | Create a case with all required fields | Case saves and required relationships are populated | Not run |
| TC-002 | Save a resolved case without resolution notes | Save is blocked if the proposed validation is implemented | Not run |
| TC-003 | Submit a case with a Billing category | Case is routed to the configured Billing destination if routing is implemented | Not run |
| TC-004 | Submit a Technical category case | Case is routed to the configured Technical destination if routing is implemented | Not run |
| TC-005 | Submit a critical case without an escalation reason | Validation or escalation behavior matches the documented business rule | Not run |
| TC-006 | Submit a case with an unknown/missing category | Documented fallback behavior occurs | Not run |
| TC-007 | Agent attempts to access a restricted record/field | Access follows the configured security model | Not run |
| TC-008 | Manager reviews team workload report | Report matches the underlying sample records | Not run |
| TC-009 | Resolved case meets the FCR definition | FCR is recorded according to the documented process | Not run |
| TC-010 | Flow handles an unexpected value or missing data | Flow follows its fault/fallback path without silent data corruption | Not run |

## Evidence policy
Never mark a test Pass until it has been executed in the target Salesforce org. Attach redacted screenshots or logs where useful. Use fictional data only.
