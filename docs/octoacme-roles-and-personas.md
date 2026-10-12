# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

---

## Developers

### Role Summary
Developers design, build, test, and deliver software components. They collaborate with product and project leads to implement features that meet acceptance criteria and quality standards.

### Responsibilities
- Implement features and fixes to meet acceptance criteria
- Write and maintain tests and documentation
- Participate in design and code reviews
- Assist in estimating and planning work
- Help identify technical risks and propose mitigations

### Goals
- Deliver reliable, maintainable code
- Reduce cycle time from idea to production
- Maintain high test coverage and observability

### Typical Communication
- Daily standups and sprint planning
- PR descriptions and code review comments
- Technical design docs when needed

---

## Product Managers

### Role Summary
Product Managers define what should be built to deliver customer and business value. They own the product vision, prioritize the backlog, and measure outcomes.

### Responsibilities
- Define problem statements and success metrics
- Prioritize the roadmap and backlog
- Collaborate with stakeholders and engineering on trade-offs
- Validate solutions through user research and metrics

### Goals
- Maximize customer value and impact
- Make clear, data-driven prioritization decisions
- Ensure product-market fit and usability

### Typical Communication
- Weekly alignment with PM and engineering leads
- Roadmap updates and stakeholder briefings
- Acceptance criteria and feature specs

---

## Project Managers

### Role Summary
Project Managers coordinate delivery activities, manage schedules, risks, and communications. They enable the team to deliver on commitments efficiently.

### Responsibilities
- Create and maintain project plans and timelines
- Manage risks, dependencies, and resource constraints
- Facilitate meetings (kickoff, planning, retrospectives)
- Ensure consistent project documentation and status reporting
- Coordinate cross-team and stakeholder communication

### Goals
- Deliver projects on time and within scope
- Minimize unplanned work and escalations
- Maintain transparency and alignment across stakeholders

### Typical Communication
- Weekly status updates and stakeholder reports
- Risk registers and decision logs
- Coordination via project boards and meeting facilitation

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

---

## Additional Personas

This section adds operational personas and clarifies responsibilities, handoffs, and escalation paths for the project management process.

| Persona | Responsibilities | Primary interactions & escalation paths |
|---|---|---|
| Program Manager (Delivery Program Lead) | Owns end-to-end program coordination across related projects, timeline alignment, consolidated status reporting, and cross-project risk mitigation. Maintains program-level roadmap and coordinates funding and priority decisions with sponsors. | Interacts with Product Owners (priorities), Delivery Leads (execution and dependencies), and Stakeholder Liaison (external reporting). Escalation: if a program-level schedule or scope risk arises, informs the sponsor and Stakeholder Liaison and coordinates mitigation with Delivery Leads and the Process Architect. |
| Delivery Lead (Project Execution Lead) | Responsible for day-to-day project execution, sprint planning, backlog grooming coordination, removing operational blockers, and ensuring sprint commitments. Tracks team capacity and delivery risks. | Works closely with the Technical Lead (task breakdown and estimates), QA Lead (test planning), and Product Owner (acceptance criteria). Escalation: architectural blockers are escalated to the Technical Lead; schedule impacts are escalated to the Program Manager. |
| Product Owner (Business Representative) | Defines product priorities, acceptance criteria, and approval of delivered scope. Owns stakeholder expectations for feature trade-offs and business value. | Coordinates with the Program Manager on roadmap trade-offs, with the UX Research Lead for user insights, and with the Delivery Lead for delivery feasibility. Escalation: unresolved priority conflicts escalate to the Program Manager or sponsor. |
| Technical Lead (Architecture / Engineering Lead) | Guides technical approach, design decisions, coding standards, and architecture governance. Reviews designs and major pull requests and mentors engineers on technical quality. | Collaborates with the Delivery Lead (estimates and implementation plans), Security Liaison (security controls), and Release Manager (deployment constraints). Escalation: complex architectural decisions escalate to an architecture review board or the Process Architect when cross-project impact exists. |
| QA Lead (Test Lead) | Defines the testing strategy, acceptance criteria verification, test automation priorities, and release test gates. Ensures test coverage and plans remediation for defects. | Works with the Delivery Lead for test scheduling, the Technical Lead for integration testing support, and the Release Manager for release criteria. Escalation: unresolved quality risks escalate to the Delivery Lead and Program Manager if they impact release dates. |
| Release Manager | Coordinates release windows, deployment approvals, rollback and contingency plans, and release communications. Validates release readiness against quality, security, and compliance gates. | Works with the Delivery Lead, engineering operations, and Stakeholder Liaison for scheduling and communications. Escalation: release-blocking issues escalate to the Program Manager and relevant Technical Lead or Security Liaison for emergency decisions. |
| Stakeholder Liaison (Business Stakeholder Manager) | Acts as the primary contact for external stakeholders and sponsors. Manages status updates, expectation alignment, and escalations from stakeholders. | Coordinates messaging and escalation with the Program Manager and Product Owner. Escalation: stakeholder escalations are routed to the Program Manager and Process Architect as needed. |
| Process Architect (Process Owner) | Owns and reviews program and process definitions, ensures consistency across process docs, approves major changes to workflows, and drives continuous improvement activities. | Works with the Documentation Owner to publish changes, the Program Manager to align process with delivery needs, and the Risk & Compliance Officer for controls. Escalation: conflicts over process or governance escalate to program sponsors. |
| Documentation Owner (Docs Steward) | Owns quality and upkeep of the docs folder, maintains templates, and coordinates updates for onboarding and operational guides. Ensures documentation is discoverable and versioned. | Works with the Process Architect on content changes, the Onboarding Coordinator for onboarding checklists, and Delivery Leads for operational how-to guides. Escalation: content disputes escalate to the Process Architect. |
| Onboarding Coordinator | Manages new-hire onboarding and role-specific orientation, tracks completion of onboarding milestones, and curates role-based learning paths. | Works with the Documentation Owner to keep onboarding materials current and with the Program Manager to align start dates. Escalation: persistent knowledge gaps escalate to the Process Architect and Delivery Lead for process-level remediation. |
| Risk & Compliance Officer | Maintains the program risk register, performs compliance checks, and ensures audit readiness. Owns risk reporting cadence and corrective actions. | Coordinates with the Program Manager for program-level risk mitigation and with the Security Liaison for security and compliance requirements. Escalation: high or severe risks are raised to sponsors and the Process Architect. |
| Security Liaison | Ensures security requirements are incorporated into design, development, and release processes. Coordinates security reviews and remediation. | Works closely with the Technical Lead, Release Manager, and Risk & Compliance Officer. Escalation: critical security issues escalate to the Program Manager and sponsors per the incident policy. |
| UX Research Lead | Represents user research findings, validates product assumptions, and advises product design decisions. Ensures user feedback is integrated into requirements. | Collaborates with the Product Owner and Documentation Owner for user-facing content and acceptance criteria. Escalation: major user-impacting findings escalate to the Product Owner and Program Manager. |

### Role entry guidance

For each persona, include:
- Responsibilities: 3–5 bullet summary of core accountabilities
- Decision authority: what decisions can be made without escalation
- Primary interactions: 2–4 roles this persona works with most often
- Escalation path: who to notify when the issue exceeds the person’s authority

### Example entry

Program Manager (Delivery Program Lead)
- Responsibilities:
  - Coordinate program delivery and align timelines across projects
  - Consolidate status, risks, and decisions for sponsors
  - Maintain the program roadmap and dependency register
- Decision authority:
  - Prioritize cross-project scheduling trade-offs in consultation with sponsors
- Primary interactions:
  - Product Owner, Delivery Lead, Stakeholder Liaison, Process Architect
- Escalation path:
  - Escalate unresolved cross-project risks to sponsors and the Process Architect; for urgent scope or funding changes, coordinate with the Stakeholder Liaison

### Implementation notes

- Add this as a new "Additional Personas" section in docs/octoacme-roles-and-personas.md.
- Keep the language concise and actionable, with emphasis on handoffs and escalation paths.
- Ensure each persona clearly explains who they collaborate with and when to escalate.
