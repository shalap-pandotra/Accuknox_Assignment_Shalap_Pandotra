# Accuknox_Assignment_Shalap_Pandotra

## Alert Triage Workflow
Cloud security tools generate a high volume of alerts across multiple cloud accounts and services. Security engineers need a way to quickly understand which alerts matter most, investigate their impact, and track resolution without being overwhelmed by noise or forced into complex remediation flows.
The challenge is not only detecting issues, but enabling effective triage, investigation, collaboration, and resolution tracking in a way that reflects real-world security workflows.

[Figma Document]([https://www.figma.com/design/mZQcco5dVowuMXU7ue8NhW/Accuknox-assignment---Shalap-Pandotra?node-id=17-2&t=fJDDGi6Tt5Xun16p-1](https://www.figma.com/design/mZQcco5dVowuMXU7ue8NhW/Accuknox-assignment---Shalap-Pandotra?node-id=0-1&t=to5hPnqjFke9wmgy-1))

## User Persona
### Primary user: Cloud / Security Engineer

Responsibilities:
* Monitor security alerts across environments
* Assess severity and potential impact
* Investigate alerts and gather context
* Coordinate remediation with service owners or infrastructure teams
* Verify fixes and mark alerts as resolved

Pain points:
* Alert fatigue and poor prioritization
* Lack of context when reviewing alerts
* Difficulty tracking ownership and resolution status
* Unclear audit trail for who handled an alert and when

## Design Overview
The proposed design focuses on a two-screen workflow that mirrors how security teams actually work:
 a triage queue for prioritization, followed by a detailed view for investigation and resolution tracking.
The system is intentionally designed as a visibility and coordination tool, not a remediation console. Technical fixes are assumed to happen outside the system, with this interface serving as the source of truth for alert status and accountability.

## Screen 1: Alert List (Triage View)
The alert list acts as a prioritized work queue.

Key features:
* Alerts grouped by day to support daily on-call and triage routines
* Severity-based visual indicators for quick scanning
* Clear resolution state using a reversible checkbox
* “Resolved by” attribution to support accountability and handoffs


### Design rationale:
Grouping alerts by day reflects how engineers typically process alerts in time-based batches, while severity indicators ensure that critical issues are not buried. Resolution is treated as a reversible state, allowing alerts to be reopened if remediation is incomplete or incorrect.

## Designs:
* [Zero State](https://www.figma.com/design/mZQcco5dVowuMXU7ue8NhW/Accuknox-assignment---Shalap-Pandotra?node-id=18-162&t=fJDDGi6Tt5Xun16p-4)
* [Triage view](https://www.figma.com/design/mZQcco5dVowuMXU7ue8NhW/Accuknox-assignment---Shalap-Pandotra?node-id=18-4&t=fJDDGi6Tt5Xun16p-4)
* [Hover tooltips](https://www.figma.com/design/mZQcco5dVowuMXU7ue8NhW/Accuknox-assignment---Shalap-Pandotra?node-id=8-75&t=fJDDGi6Tt5Xun16p-4)
* [Resolved State](https://www.figma.com/design/mZQcco5dVowuMXU7ue8NhW/Accuknox-assignment---Shalap-Pandotra?node-id=14-2&t=fJDDGi6Tt5Xun16p-4)
* [Sorting Options](https://www.figma.com/design/mZQcco5dVowuMXU7ue8NhW/Accuknox-assignment---Shalap-Pandotra?node-id=15-404&t=fJDDGi6Tt5Xun16p-4)
* [Sorted State](https://www.figma.com/design/mZQcco5dVowuMXU7ue8NhW/Accuknox-assignment---Shalap-Pandotra?node-id=15-582&t=fJDDGi6Tt5Xun16p-4)

## Screen 2: Alert Details (Investigation & Resolution)
The detail view provides all necessary context to investigate and close an alert.

Key features:
* Plain-English explanation of the issue and its potential impact
* Clear display of affected resources and timestamps
* Internal discussion/comments for collaboration and escalation
* Explicit resolution controls and audit trail (who resolved the alert and when)


### Design rationale:
This view focuses on understanding and coordination rather than direct remediation. By surfacing risk context and supporting team discussion, the design reflects real-world workflows where fixes are applied externally and verified before an alert is resolved.

## Designs:
* [Details View - unresolved](https://www.figma.com/design/mZQcco5dVowuMXU7ue8NhW/Accuknox-assignment---Shalap-Pandotra?node-id=20-436&t=fJDDGi6Tt5Xun16p-4)
* [Details View - resolved](https://www.figma.com/design/mZQcco5dVowuMXU7ue8NhW/Accuknox-assignment---Shalap-Pandotra?node-id=24-39&t=fJDDGi6Tt5Xun16p-4)

## Success Metrics
The effectiveness of this design could be measured by:
* Time to first action on newly detected alerts
* Percentage of alerts resolved vs reopened
* Reduction in unresolved critical alerts over time
* Clarity of ownership and resolution accountability

[Assignment PDF](Accuknox_Assignment_Shalap_Pandotra.pdf)

