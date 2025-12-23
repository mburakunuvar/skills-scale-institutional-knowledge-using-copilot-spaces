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
- Assess: estimate impact and likelihood
- Mitigate: reduced via actions, contingency plans
- Monitor: review at weekly syncs and update status

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
- Triage summary
- Actions being taken
- Expected timeline
- Post-incident blameless retrospective scheduled

## Escalation Paths
- Team-level -> PM -> Product Lead -> Sponsor
- For security incidents, follow the security incident runbook and notify Security on-call

## Cross-Team Dependency Management

Effective cross-team coordination is critical to project success. Use this framework to identify, track, and resolve dependencies with other teams.

### Identifying Dependencies
During planning and execution:
- Map out which features or tasks require work from other teams
- Document dependencies in the project board with clear labels
- Add to the risk register with Impact and Likelihood assessment
- Identify the dependency owner and contact from the other team

### Dependency Tracking Template
For each cross-team dependency, document:
- **Dependency ID**: Unique identifier (e.g., DEP-001)
- **Description**: What is needed and why
- **Dependent Team**: Which team needs to deliver this
- **Contact**: Primary point of contact on the other team
- **Target Date**: When you need this delivered
- **Status**: Not Started / In Progress / Blocked / Complete
- **Impact if Delayed**: How this affects your project timeline
- **Last Updated**: Date of last status check

### Regular Coordination
- **Weekly check-ins**: PM or designated owner follows up with dependency contacts
- **Status updates**: Request and document status in the risk register or project board
- **Proactive communication**: Notify dependent teams early of any changes to your timeline or requirements
- **Escalation triggers**: If status hasn't been updated in 1 week or dependency is at risk

### When Blocked by Another Team

Follow this escalation path to resolve blockers:

**Level 1: Direct Coordination (Days 1-3)**
- Reach out directly to the dependency contact
- Clearly explain the blocker and its impact on your timeline
- Propose solutions or alternatives if possible
- Document the blocker in your risk register and standup

**Level 2: Manager Escalation (Days 4-7)**
- If no resolution, escalate to both PMs (yours and theirs)
- PMs should sync to prioritize, negotiate timeline, or identify workarounds
- Update stakeholders on the blocker and revised timeline if needed
- Document escalation and agreed-upon resolution path

**Level 3: Leadership Escalation (Days 8+)**
- If still blocked, escalate to Product Leads or Sponsors
- Provide clear impact analysis and alternative options
- Leadership should align on priority trade-offs across teams
- Communicate resolution and updated plans to all stakeholders

### Dependency Coordination Template

Use this template for weekly cross-team dependency updates:

```
**Weekly Dependency Update - [Date]**

**Dependencies on Other Teams:**
- DEP-ID | Team | Description | Status | Target Date | Blocker (if any)
- DEP-001 | Platform Team | API endpoint for user data | In Progress | 2025-01-15 | None
- DEP-002 | Data Team | Analytics schema update | Blocked | 2025-01-10 | Awaiting schema review

**Updates from Our Team (impacting others):**
- DEP-003 | Our Team → Mobile Team | Authentication service | Complete | 2025-01-05 | Deployed to staging

**Action Items:**
- [ ] Follow up with Data Team on schema review (Owner: PM)
- [ ] Notify Mobile Team of auth service availability (Owner: Dev Lead)

**Escalations Needed:**
- DEP-002 - blocked for 5 days, escalating to PM level
```

### Best Practices
- **Early identification**: Flag dependencies during planning, not mid-sprint
- **Clear requirements**: Provide detailed specs and acceptance criteria to dependent teams
- **Buffer time**: Add buffer to your timeline for dependency delays
- **Bi-directional communication**: Share your status with teams depending on you
- **Celebrate coordination wins**: Recognize teams that deliver dependencies on time
