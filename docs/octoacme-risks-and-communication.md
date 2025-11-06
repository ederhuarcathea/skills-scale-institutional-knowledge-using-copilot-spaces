# OctoAcme — Risk Management & Communication

## Purpose
Explain how to identify, manage, and communicate risks and dependencies.

## Risk Register
Maintain a simple table with:
- ID
- Description
- Impact (High/Med/Low)
- Likelihood (High/Med/Low)
- Owner
- Mitigation plan
- Status

## Risk Lifecycle
- Identify: during planning and ongoing execution
- Assess: estimate impact and likelihood with input from technical leads and SREs
- Mitigate: reduced via actions, contingency plans
- Monitor: review at weekly syncs and update status

### SRE Involvement in Risk Management
- **Site Reliability Engineers (SREs)** play a critical role in identifying and mitigating technical risks:
  - Assess infrastructure and scalability risks during planning
  - Define reliability requirements and Service Level Objectives (SLOs)
  - Monitor system health and alert on potential issues
  - Lead incident response and coordinate recovery efforts
  - Conduct blameless postmortems to prevent recurrence

## Stakeholder Communication
- Identify stakeholder groups and communication needs (e.g., engineering, sales, support)
- Provide regular updates (weekly or milestone-based)
- Use a single source of truth (project README or release doc) for status

## Communication Templates
Weekly Status Template:
- Progress this week:
- Next steps:
- Risks & blockers:
- Ask / decisions needed:

Incident Communication
- Triage summary (coordinated by SRE on-call)
- Actions being taken
- Expected timeline
- Post-incident blameless retrospective scheduled (facilitated by SRE and Scrum Master)

## Escalation Paths
- Team-level -> PM -> Product Lead -> Sponsor
- For security incidents, follow the security incident runbook and notify Security on-call

## Risk Management Checklist Example
When identifying a new technical risk:
- [ ] Document risk in Risk Register with ID, description, and initial assessment
- [ ] Consult with SRE for infrastructure/reliability impact assessment
- [ ] Identify risk owner (PM, Tech Lead, or SRE)
- [ ] Define mitigation plan with specific actions and timeline
- [ ] Add monitoring or alerts if applicable (SRE to implement)
- [ ] Review risk status in weekly PM sync
- [ ] Update stakeholders if risk level is High
