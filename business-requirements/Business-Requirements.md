# Business Requirements — Smart Customer Support & Resolution Hub

**Status:** Initial design  
**Business:** NovaCart (fictional e-commerce retailer)

## 1. Problem statement
Support requests may be categorized inconsistently, assigned manually, escalated late, and handled without a consistent view of customer and product context. Managers also need reliable reporting on workload and outcomes.

## 2. Business goals
1. Standardize case categorization and priority decisions.
2. Reduce avoidable manual assignment through rules-based automation.
3. Make ownership and escalation more visible.
4. Help agents find approved troubleshooting guidance.
5. Measure case volume, aging, resolution outcomes, and customer feedback.

These are project goals, not measured outcomes. No performance improvement is claimed at this stage.

## 3. Stakeholders and personas
- **Support Agent:** investigates and resolves customer cases.
- **Support Manager:** monitors workload, reassigns work, and handles escalations.
- **Knowledge Manager:** maintains approved support articles.
- **Salesforce Administrator:** manages configuration, access, automation, and reporting.
- **Customer:** submits a support request and receives updates.

## 4. In-scope capabilities
- Standard Salesforce records for customer and case context.
- Case classification and priority design.
- Validation and data-quality controls.
- Role/permission/sharing design.
- Flow-based routing support, notifications, and escalation.
- Queues and Omni-Channel design, subject to edition and license availability.
- Knowledge, reports, dashboards, and test evidence.
- Agentforce and Slack as later, optional extensions.

## 5. Out of scope for the initial release
- Real payment processing or refund execution.
- Connection to a real e-commerce order-management system.
- Use of real customer personal data.
- Production deployment or customer-facing AI without security and policy review.
- Data 360 implementation until org access, licensing, and use case are confirmed.

## 6. Functional requirements
| ID | Requirement | Priority | Acceptance summary |
|---|---|---|---|
| FR-01 | Store customer issues as Cases | Must | A test case can be created and associated with appropriate customer records. |
| FR-02 | Classify cases consistently | Must | Approved category and subcategory values are available. |
| FR-03 | Validate resolution information | Must | A case cannot be marked resolved without required resolution details, if that rule is implemented. |
| FR-04 | Determine a suggested support team | Must | Test cases map to the intended queue/team using documented rules. |
| FR-05 | Flag urgent or aging cases | Should | Cases meeting configured criteria are identified and escalated. |
| FR-06 | Provide agent Knowledge resources | Should | Agents can find relevant approved articles in the configured experience. |
| FR-07 | Report service performance | Should | Reports show agreed measures using documented definitions. |
| FR-08 | Explore AI-assisted service | Later | Agentforce use case is tested only if the required features and licenses are available. |

## 7. Non-functional requirements
- Apply least-privilege access and test access as different personas.
- Use fictional/sample data only.
- Keep configuration names consistent and documented.
- Record test steps, expected results, observed results, and evidence.
- Do not claim performance gains unless they are measured and reproducible.
- Verify feature availability and release-specific behavior in the target org.

## 8. Success measures to evaluate
- Percentage of test cases routed to the expected team.
- Time required to assign a test case before and after automation.
- Percentage of cases with required fields completed.
- Number of test cases passing validation and security scenarios.
- Report accuracy against the test dataset.

Targets will be set after a baseline and test dataset are defined.
