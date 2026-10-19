# Security Architecture — Initial Design

**Status:** Proposed design; must be validated in the target org.

## 1. Security principles
- Least privilege.
- Separate object permissions, field-level security, and record-level sharing.
- Use permission sets and permission set groups for additive access where appropriate.
- Use roles to support record access through hierarchy where configured; a role does not automatically grant all object permissions.
- Test with representative users rather than relying only on an administrator session.

## 2. Personas
| Persona | Intended access |
|---|---|
| Support Agent | Work assigned/accessible cases; view relevant customer context; use approved service tools |
| Support Manager | Review team workload; handle escalations; access operational reports |
| Knowledge Manager | Create, review, and maintain support articles if Knowledge is enabled |
| Salesforce Administrator | Configure and troubleshoot the solution |

## 3. Proposed access components
- **Profile:** minimum baseline and required default settings.
- **Permission Sets:** additional object, field, app, and system permissions.
- **Permission Set Groups:** bundle permissions for a job function when this simplifies administration.
- **Role Hierarchy:** support manager visibility where applicable.
- **Organization-Wide Defaults:** choose the most restrictive practical baseline based on the use case and license.
- **Sharing Rules / manual sharing / teams:** expand access only where justified.

## 4. Important implementation cautions
- Do not blindly set Case OWD to Private without checking ownership, queue behavior, manager access, automation context, reporting requirements, and org-wide constraints.
- Permission sets grant permissions; they do not by themselves grant access to every record.
- Review field-level security separately from page layouts.
- Do not create or modify production access as part of this portfolio without authorization.
- Exact capabilities depend on org edition, licenses, and enabled features.

## 5. Security test plan
1. Verify an agent can perform only intended case actions.
2. Verify a manager can access the cases and reports needed for their role.
3. Verify a Knowledge Manager can maintain articles but does not receive unrelated administrative privileges.
4. Verify restricted fields are not exposed to unauthorized users.
5. Verify a user cannot access a case merely because it appears in a navigation item; check actual record sharing.

## 6. Status
No access model is claimed to be configured yet. Record actual Setup screenshots and test evidence after implementation.
