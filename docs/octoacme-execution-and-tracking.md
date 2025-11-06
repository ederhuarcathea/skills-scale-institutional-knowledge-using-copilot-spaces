# OctoAcme — Execution & Tracking

## Purpose
Guidance for managing day-to-day execution and tracking progress toward project milestones.

## Team Rhythm
- Daily standups (15 min) — facilitated by Scrum Master, focus on progress, blockers, dependencies
- Weekly delivery sync — show progress, updates, and flagged risks
- Demo/Review at the end of each sprint or milestone — facilitated by Scrum Master

### Scrum Master's Role in Team Rhythm
- Facilitates all agile ceremonies and keeps them timeboxed
- Tracks action items and ensures follow-through
- Identifies and escalates impediments that block team progress
- Coaches team on agile best practices and self-organization
- Protects team from external interruptions during sprint execution

## Workflows
- Use the project board (e.g., GitHub Projects) with columns: Backlog, Ready, In Progress, In Review, QA, Done
- Pull Request workflow:
  - Small PRs (<= 400 lines when possible)
  - Include issue link and acceptance criteria in PR description
  - Run automated tests and linting in CI before requesting review
  - Require at least one approval before merging (or team-defined policy)

## Quality & Testing
- Unit tests for new logic
- Integration tests where applicable
- End-to-end smoke tests for critical flows before release
- Security scanning in CI
- Manual QA for feature acceptance when needed

## Reporting & Metrics
- Track velocity and burndown (Scrum Master maintains sprint metrics)
- Monitor success metrics identified in the Project One-pager
- Use dashboards for key signals (errors, latency, usage) — SRE provides observability
- Report team health and improvement trends (Scrum Master)

## Blocker Escalation
- Level 1: Team-level triage in daily standup (Scrum Master facilitates)
- Level 2: PM escalates to Product Lead and dependent teams (Scrum Master may assist)
- Level 3: Sponsor-level escalation for business-impacting issues

## Execution Checklist
- [ ] Branching and PR conventions documented in repo
- [ ] CI configured for tests and lint
- [ ] Regular demos scheduled
- [ ] Risk register updated weekly

## Example: Role Collaboration During Sprint Execution

**Scenario**: A team is implementing a new user dashboard feature during a 2-week sprint.

**Day 1 (Sprint Start)**:
- Scrum Master facilitates sprint planning with prioritized backlog
- UX Designer presents finalized wireframes and design specs
- Developers estimate tasks and commit to sprint goal
- SRE reviews infrastructure requirements and monitoring needs

**Day 3 (Development)**:
- Developer encounters design ambiguity; UX Designer clarifies in Slack
- Technical Writer begins drafting user guide based on design specs
- SRE sets up staging environment and monitoring dashboards

**Day 7 (Mid-Sprint)**:
- Daily standup: Developer reports API integration blocker
- Scrum Master escalates to PM for cross-team coordination
- SRE helps debug performance issue in staging

**Day 10 (Pre-Release)**:
- QA completes acceptance testing
- Technical Writer finalizes release notes with PM input
- SRE validates deployment checklist and rollback plan

**Day 14 (Sprint End)**:
- Scrum Master facilitates demo to stakeholders
- Business Analyst validates that acceptance criteria meet business needs
- Team conducts retrospective to identify improvements
