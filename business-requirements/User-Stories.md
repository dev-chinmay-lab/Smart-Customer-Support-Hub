# User Stories and Acceptance Criteria

**Status:** Proposed backlog

## US-01 — Create a support case
**As a** support agent, **I want** to record a customer's issue with a category, priority, and relevant customer/product context, **so that** the request can be tracked consistently.

**Acceptance criteria**
- A case can be created with the required fields.
- Category and priority use controlled values.
- Required-field behavior is verified with positive and negative tests.

## US-02 — Route a case to the appropriate team
**As a** support manager, **I want** cases to be assigned based on their category, **so that** the correct team can investigate them.

**Acceptance criteria**
- Each in-scope category has a documented destination.
- Test cases are assigned to the expected queue or owner.
- An unrecognized or missing category follows a documented fallback path.

## US-03 — Escalate urgent cases
**As a** support manager, **I want** urgent cases to be flagged and brought to the team's attention, **so that** they can be reviewed promptly.

**Acceptance criteria**
- Escalation criteria are documented.
- A qualifying test case is flagged and the intended notification/action occurs.
- A non-qualifying case does not trigger the escalation path.

## US-04 — Capture resolution details
**As a** support manager, **I want** resolved cases to include resolution details, **so that** outcomes can be audited and analyzed.

**Acceptance criteria**
- The configured validation prevents incomplete resolution where applicable.
- A complete resolution can be saved.
- Both scenarios are documented in test results.

## US-05 — Protect customer information
**As a** Salesforce administrator, **I want** access to follow job responsibilities, **so that** users only receive the access they need.

**Acceptance criteria**
- Persona permissions are documented.
- Object/field permissions and record sharing are reviewed separately.
- Access tests are run with appropriate test users when available.

## US-06 — Monitor service performance
**As a** support manager, **I want** reports on case volume, status, priority, aging, and resolution, **so that** I can identify workload and bottlenecks.

**Acceptance criteria**
- Every KPI has a written definition.
- Report totals are checked against the sample records.
- Dashboard screenshots are added only after the dashboard exists in Salesforce.
