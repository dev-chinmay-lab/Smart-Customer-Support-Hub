# Support Operations — KPI Definitions

**Status:** Proposed metrics; definitions must be agreed before reports are built.

| KPI | Proposed definition | Important caveat |
|---|---|---|
| Open Cases | Count of cases not in the agreed closed statuses at report time | Define status values consistently. |
| Critical Cases | Count of cases whose Priority equals Critical and that are not closed | Depends on configured priority values. |
| Cases Created | Count of cases created during a selected period | State the reporting date field and time zone. |
| Average Resolution Time | Average elapsed time from case creation to resolution for resolved cases | Define whether business hours or elapsed hours are used. |
| First Contact Resolution (FCR) | Resolved cases meeting the agreed first-contact definition divided by eligible resolved cases | Do not treat a checkbox as proof unless the process defines how it is set. |
| Escalation Rate | Escalated cases divided by eligible cases in the same period | Define numerator, denominator, and period. |
| Agent Workload | Open cases by current owner/queue | Reassignment can affect historical comparisons. |
| CSAT | Average or distribution of customer survey scores for responses received | Requires a feedback collection mechanism and enough data. |

## Dashboard plan
1. **Support Operations:** open cases, critical cases, cases created, aging, resolution time.
2. **Team Workload:** open cases by owner/queue, cases resolved, aging distribution.
3. **Quality & Experience:** FCR, escalation rate, CSAT when the data collection process exists.

## Reporting integrity
- Do not invent KPI values.
- Use sample records and clearly label test/demo data.
- Verify report totals against the underlying records.
- Add screenshots only after the reports or dashboards are actually built.
