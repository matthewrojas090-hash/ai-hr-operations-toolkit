# AI Employee Onboarding Plan Builder

Create a structured, role-specific onboarding plan from approved company information—without inventing policies, expectations, or employee details.

## What this tool does

This workflow helps HR teams and managers:

- Organize preboarding responsibilities
- Build a practical first-week schedule
- Create 30-, 60-, and 90-day milestones
- Assign clear owners across HR, IT, the manager, and the employee
- Connect learning activities to the employee’s role
- Identify missing access, training, or policy information
- Establish consistent manager check-ins
- Define evidence that onboarding is progressing
- Give the employee a clear and welcoming experience

AI organizes approved information. HR and the employee’s manager remain responsible for reviewing and approving the plan.

## What you need

Prepare only the information necessary to create the plan:

- Job title and department
- Job description
- Role level
- Work arrangement, such as onsite, hybrid, or remote
- Approved company onboarding requirements
- Required training
- Systems and access needed
- Important stakeholders
- Manager expectations
- Role-specific responsibilities
- Verified 30-, 60-, and 90-day expectations
- Existing onboarding templates
- Known deadlines or dependencies

Do not provide medical information, accommodation requests, protected characteristics, compensation records, government identification numbers, personal contact information, employee-relations information, or other sensitive data.

## Input template

```
ROLE INFORMATION

Job title:
Department:
Role level:
Work arrangement:
Start date, if needed for planning:
Job description or approved role summary:

APPROVED EXPECTATIONS

Important responsibilities:
First 30-day expectations:
First 60-day expectations:
First 90-day expectations:
How success will be reviewed:
Expectations that are still unclear:

REQUIRED LEARNING

Company orientation:
Policy training:
Compliance training:
Role-specific training:
Required certifications:
Existing learning materials:

SYSTEMS AND ACCESS

Systems required:
Equipment required:
Security or access requirements:
Who approves each request:
Known access lead times:

PEOPLE AND SUPPORT

Manager:
Onboarding partner or buddy:
Important stakeholders:
Teams the employee should understand:
Regular meetings:
Escalation contact:

COMPANY REQUIREMENTS

Approved onboarding checklist:
Relevant policies or procedures:
Required forms:
Existing onboarding template:
Known deadlines or dependencies:

PRIVACY CHECK

Information removed before using AI:
Information that must not appear in the output:
```

## Copy-and-paste AI prompt

```
You are helping an HR team and manager organize an employee onboarding plan.

Use only the information provided below. Do not invent company policies, legal requirements, training, performance expectations, employee details, deadlines, system access, or success measures.

Do not provide legal conclusions or make employment decisions. If important information is missing, label it “Needs human confirmation.”

Source information:

[PASTE THE COMPLETED INPUT TEMPLATE]

Create the following:

### 1. Input-quality review

Separate the source material into:

- Verified information
- Missing information
- Conflicting information
- Information requiring HR confirmation
- Information requiring manager confirmation
- Private or unnecessary information that should be removed

### 2. Preboarding checklist

Create a checklist covering only applicable, verified tasks.

Use these columns:

| Task | Owner | Due point | Dependency | Status |
|---|---|---|---|---|

Possible owners include HR, the manager, IT, workplace operations, security, learning and development, and the employee.

Do not assign an owner when ownership was not supplied. Mark it “Needs assignment.”

### 3. First-day plan

Create a welcoming and practical first-day schedule.

Include:

- Orientation
- Manager connection
- Team introductions
- Equipment and systems check
- Essential policy or security information
- Time for questions
- End-of-day check-in

Do not overload the first day with every available training activity.

### 4. First-week plan

Create a five-day plan that balances:

- Company orientation
- Role learning
- Stakeholder introductions
- Systems access
- Required training
- Independent review time
- Manager check-ins
- Questions and reflection

Label any activity that depends on information that has not been confirmed.

### 5. 30-, 60-, and 90-day plan

Create this table:

| Period | Learning priorities | Expected activities | Evidence of progress | Support needed | Owner |
|---|---|---|---|---|---|

Use only approved expectations.

Do not transform onboarding milestones into automatic performance ratings. Do not describe an employee as successful, unsuccessful, high potential, or underperforming.

### 6. Role-specific learning path

Organize required learning into:

1. Company knowledge
2. Team knowledge
3. Role knowledge
4. Systems and tools
5. Policies and procedures
6. Stakeholder knowledge
7. Optional development

For every item, state whether it is:

- Required
- Recommended
- Needs confirmation

### 7. Manager enablement guide

Create a manager checklist covering:

- What to prepare before the employee starts
- What to explain during the first week
- Questions to ask during check-ins
- Information the employee may need
- Obstacles the manager should help remove
- Topics requiring HR support

Include suggested check-ins at the end of the first day, first week, 30 days, 60 days, and 90 days.

### 8. Responsibility table

Create this table:

| Activity | HR | Manager | IT or Operations | Employee | Needs confirmation |
|---|---|---|---|---|---|

Do not assume responsibility that was not established in the source information.

### 9. Onboarding risks

Identify operational risks such as:

- Delayed system access
- Missing equipment
- Unclear role expectations
- Missing training
- Unassigned responsibilities
- Scheduling conflicts
- Missing stakeholder introductions
- Dependencies without owners

For each risk, provide:

- Supporting evidence
- Potential impact
- Recommended human follow-up
- Owner, if known

Do not diagnose the employee or speculate about motivation, personality, commitment, or future performance.

### 10. Employee-facing plan

Create a concise, welcoming version of the plan for the employee.

Use clear language and explain:

- What will happen before the start date
- What to expect during the first week
- The main learning priorities
- Who can provide support
- When check-ins will occur
- Which details are still being confirmed

Do not include private HR notes or internal risk discussions.

### 11. Final verification checklist

Provide a checklist for HR and the manager to confirm:

- All policies are current
- Every required task has an owner
- Dates and deadlines are correct
- System-access requirements are accurate
- Milestones match the approved role expectations
- Private information was removed
- Employee-facing information is appropriate to share
- Accessibility and accommodation processes are handled through approved HR channels
- A qualified person approved the final plan

Finish with this reminder:

“AI organized the supplied information. HR and the manager must verify the plan, correct missing or inaccurate details, and remain accountable for the employee’s onboarding experience.”
```

## Fictional example

### Source information

```
Job title: People Operations Coordinator
Department: People Operations
Role level: Individual contributor
Work arrangement: Hybrid

Important responsibilities:
Coordinate employee documentation, maintain approved HR process guides,
schedule onboarding activities, and respond to routine employee requests.

First 30-day expectations:
Complete required training, learn the HR request process, and observe
two onboarding sessions.

First 60-day expectations:
Coordinate onboarding logistics with manager review.

First 90-day expectations:
Independently coordinate standard onboarding logistics using approved
procedures, with escalation support available.

Required systems:
Fictional HRIS, ticketing system, document repository, and scheduling tool.

Known risk:
HRIS access can take five business days.

Important stakeholders:
People Operations manager, IT service desk, payroll partner, recruiters,
and workplace operations.
```

### Example onboarding milestones

| Period | Learning priorities | Expected activities | Evidence of progress | Support needed | Owner |
|---|---|---|---|---|---|
| First 30 days | Approved HR processes and systems | Complete training and observe two onboarding sessions | Training completion and observation notes | System access and manager coaching | Manager and HR |
| Days 31–60 | Onboarding coordination | Coordinate logistics with manager review | Completed checklist reviewed by manager | Feedback and escalation guidance | Manager |
| Days 61–90 | Standard process ownership | Coordinate a standard onboarding process using approved procedures | Completed process checklist | Access to current procedures | Employee and manager |

This fictional example establishes learning and operating milestones. It does not make a performance rating or employment decision.

## Human review guidance

Before using the plan:

1. Confirm that every policy and procedure is current.
2. Ask the manager to approve role expectations and milestones.
3. Confirm task ownership with HR, IT, and operations.
4. Verify that the employee-facing version contains no internal notes.
5. Replace every “Needs human confirmation” item.
6. Review accessibility through the company’s approved process.
7. Keep the final plan flexible as business needs and employee questions develop.

## Responsible-AI and privacy safeguards

- Use role information, not protected characteristics.
- Do not enter health, disability, accommodation, immigration, compensation, investigation, or employee-relations information.
- Remove unnecessary employee identifiers.
- Do not ask AI to determine whether an employee is performing successfully.
- Do not treat onboarding activity as an automatic performance score.
- Do not let AI invent policies, legal requirements, deadlines, or expectations.
- Verify the output against current company materials.
- Keep HR and the manager responsible for final decisions.
- Use an employer-approved AI system when company information is involved.
- Follow applicable retention, security, and access requirements.

## Intended impact

This workflow is designed to reduce manual planning, improve ownership, and create a more consistent onboarding experience. Actual time savings and results should be measured before making performance claims.

Matthew Rojas previously helped reduce recruiter onboarding from eight weeks to four. That is prior professional experience and is not a guaranteed result of this resource.

## Disclaimer

This resource provides general organizational support. It is not legal, employee-relations, accommodation, or performance-management advice. Organizations should adapt it to their approved policies and have qualified HR, privacy, security, and legal professionals review its use.

All people, organizations, systems, and examples are fictional.
