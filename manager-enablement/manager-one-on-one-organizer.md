# AI Manager One-on-One Organizer

Turn approved goals, prior commitments, and de-identified notes into a focused manager–employee conversation and an accurate follow-up record.

## What this tool does

This workflow helps managers and HR teams:

- Prepare a balanced one-on-one agenda
- Revisit commitments from the previous meeting
- Connect discussion topics to approved role expectations and goals
- Separate facts, employee statements, manager observations, and assumptions
- Capture decisions, owners, and due dates
- Identify questions that require HR or leadership guidance
- Create an employee-facing recap for confirmation
- Maintain continuity without turning routine meetings into surveillance or automated performance ratings

AI organizes information. The manager and employee remain responsible for the conversation, corrections, commitments, and next steps.

## Appropriate use

Use this workflow for routine manager enablement, such as:

- Weekly or biweekly one-on-ones
- Goal and priority alignment
- Workload and dependency discussions
- Development planning
- Recognition and feedback
- Support requests
- Follow-up on agreed actions

Do not use this workflow to conduct an investigation, make a termination or disciplinary decision, diagnose health or performance, determine accommodations, or replace an approved employee-relations process.

## What you need

Use only information that is relevant and approved for the conversation:

- Employee role or job family
- Current approved goals or priorities
- Prior action items
- Project updates supplied by the employee or manager
- Known deadlines and dependencies
- Development interests voluntarily shared for this purpose
- Recognition or feedback that can be supported with examples
- Questions the manager or employee wants to discuss

Do not enter medical or disability information, accommodation details, protected characteristics, compensation records, investigation information, complaints, leave details, immigration information, private contact information, or confidential employee-relations facts into an external AI system.

## Input template

Use a role label or employee-approved identifier instead of a full name when possible. Write `Unknown` when information has not been confirmed.

```text
MEETING CONTEXT

Employee label:
Role or job family:
Meeting date:
Meeting type: Weekly / Biweekly / Monthly / Other
Purpose of this meeting:

APPROVED PRIORITIES

Current goals or priorities:
Known deadlines:
Approved success measures:
Changes since the previous meeting:
Information that still needs confirmation:

PRIOR COMMITMENTS

Previous employee actions:
Previous manager actions:
Completed items:
Open items:
Blocked items:

DISCUSSION INPUTS

Employee-submitted topics:
Manager-submitted topics:
Project updates:
Workload or dependency questions:
Recognition supported by examples:
Feedback supported by examples:
Development topics voluntarily shared:
Decisions needed:

SOURCE AND ACCURACY NOTES

Facts supported by a source:
Employee statements that need confirmation:
Manager observations that need discussion:
Assumptions that should not be presented as facts:
Information removed for privacy:
Topics that require HR guidance:
```

## Prompt 1: Prepare the meeting

```text
You are helping a manager prepare for a routine one-on-one conversation.

Use only the information supplied below. Do not invent employee statements, goals, deadlines, commitments, results, concerns, motives, health information, or performance conclusions.

Do not infer protected characteristics, diagnose the employee, calculate a performance score, recommend discipline or termination, or make an employment decision. If the information suggests a policy, accommodation, leave, complaint, safety, or employee-relations question, label it “Refer to the appropriate HR process” without offering a legal conclusion.

Source information:

[PASTE THE COMPLETED INPUT TEMPLATE]

Create the following:

### 1. Information-quality review

Separate the source information into:

- Confirmed facts
- Employee-provided statements
- Manager observations to discuss
- Missing or unclear information
- Assumptions that must not be presented as facts
- Private or unnecessary details that should be removed
- Topics that should be handled through an approved HR process

### 2. Proposed agenda

Create a 30-minute agenda with suggested time ranges. Include, when supported:

1. Employee priorities and questions
2. Recognition or progress
3. Current goals and work
4. Obstacles, workload, or dependencies
5. Feedback and development
6. Decisions and action items

Do not place sensitive manager-only notes in the employee-facing agenda. Do not overload the meeting. Place the employee’s submitted topics near the beginning.

### 3. Prior-commitment review

Create this table:

| Commitment | Owner | Original due date | Confirmed status | Evidence | Follow-up needed |
|---|---|---|---|---|---|

Do not mark an item complete unless the supplied information confirms completion.

### 4. Manager preparation questions

Suggest up to eight open-ended questions grounded in the supplied information. Include questions that help the manager understand:

- What is progressing
- What is blocked
- Whether priorities remain clear
- What support is needed
- Which dependencies require action
- What the employee wants to learn or develop
- What should change before the next meeting

Avoid leading questions, personality judgments, questions about protected information, and questions that assume poor intent.

### 5. Feedback preparation

For each supported feedback or recognition topic, organize:

- Specific situation or work example
- Observable action or result
- Relevant goal, expectation, or impact
- Question inviting the employee’s perspective
- Possible support or next step
- Missing evidence that must be confirmed

Keep observations behavioral and job-related. Do not label personality, attitude, potential, loyalty, or cultural fit.

### 6. Decisions and support needed

List:

- Decisions the manager can make
- Decisions requiring leadership input
- Support the manager may need to provide
- Dependencies requiring another team
- Questions requiring HR guidance
- Information that should be confirmed before the meeting

### 7. Employee-facing agenda

Create a concise agenda the manager can share before the meeting. Include the purpose, main topics, and an invitation for the employee to add or reorder topics.

Do not include private manager notes, risk labels, speculation, or HR-only information.

### 8. Human-review checklist

Ask the manager to confirm:

- The agenda includes the employee’s topics
- Every goal and deadline is current
- Feedback is supported by specific examples
- Observations are separated from assumptions
- Private information was removed
- Sensitive topics are routed through approved HR channels
- The employee-facing agenda is appropriate to share
- The manager, not AI, owns the conversation

Finish with this reminder:

“AI organized the information provided. The manager must verify the facts, listen to the employee’s perspective, correct the record, and remain accountable for the conversation and all employment decisions.”
```

## Prompt 2: Organize the follow-up

Use this prompt after the meeting with de-identified notes. Do not upload a recording or transcript unless company policy, participant notice or consent requirements, security controls, and the approved AI system permit it.

```text
You are helping organize a factual follow-up from a routine manager–employee one-on-one.

Use only the notes provided. Do not invent statements, agreements, emotions, performance conclusions, dates, owners, or outcomes. Do not treat silence as agreement.

Do not infer protected characteristics, diagnose performance or health, recommend discipline, or make employment decisions. Clearly label conflicting or incomplete information.

Approved goals and pre-meeting agenda:

[PASTE THE VERIFIED GOALS AND AGENDA]

De-identified meeting notes:

[PASTE THE NOTES]

Create the following:

### 1. Accuracy and privacy check

Identify:

- Confirmed statements
- Statements that need confirmation
- Conflicting information
- Missing owners or dates
- Private or unnecessary information to remove
- Topics that should be routed through an approved HR process

### 2. Factual meeting summary

Summarize the topics discussed without assigning motives, emotions, agreement, or blame that the notes do not support.

Separate:

- Employee-reported updates
- Manager-provided information
- Jointly confirmed decisions
- Open questions
- Items needing correction or confirmation

### 3. Goal and priority updates

Create this table:

| Goal or priority | Confirmed update | Evidence or source | Change agreed | Uncertainty | Next review |
|---|---|---|---|---|---|

Do not create a performance rating or convert incomplete activity data into a judgment about the employee.

### 4. Action register

Create this table:

| Action | Owner | Due date | Dependency | Status | Confirmation needed |
|---|---|---|---|---|---|

Use “Needs confirmation” for any owner or date not clearly agreed in the notes.

### 5. Support and escalation items

Organize supported items into:

- Manager support
- Cross-functional dependency
- Leadership decision
- HR process guidance
- No immediate action

Do not recommend an employment action. Explain only the factual reason each item needs follow-up.

### 6. Employee-facing recap

Draft a concise recap that includes:

- Main topics discussed
- Confirmed decisions
- Action items and owners
- Confirmed dates
- Open questions
- An invitation to correct or clarify the record

Do not include private manager notes, speculation, hidden ratings, or HR-only information.

### 7. Next-meeting starter

Create a short list of items to revisit at the next one-on-one, based only on open commitments and confirmed priorities.

### 8. Human confirmation

Finish with a checklist asking the manager to confirm:

- The recap reflects what was actually discussed
- The employee’s statements are represented accurately
- Agreements are not inferred from silence
- Every owner and due date was confirmed
- Private or sensitive details were removed
- HR-sensitive topics are handled outside this routine recap
- The employee is invited to correct the record
- The manager approves the final version before sharing or storing it

Finish with this reminder:

“This draft is an organizational aid, not an official performance determination. Verify it with the meeting participants and follow approved HR, privacy, retention, and documentation practices.”
```

## Fictional example

### Source information

```text
Employee label: Team Member A
Role or job family: People Operations Specialist
Meeting type: Biweekly

Current approved priorities:
- Update the approved onboarding checklist by October 2
- Coordinate two scheduled onboarding sessions
- Document common HR service requests using the existing template

Prior employee action:
- Draft the first five service-request entries by September 18

Prior manager action:
- Confirm the current policy owners by September 17

Confirmed update:
- Team Member A completed five draft entries and requested policy-owner review

Known dependency:
- The current security-access procedure is awaiting confirmation from IT

Employee-submitted topic:
- Wants practice leading part of the next onboarding session

Recognition supported by an example:
- The employee identified two conflicting steps in the onboarding checklist and paused publication for review
```

### Example agenda

| Time | Topic | Purpose |
|---:|---|---|
| 5 minutes | Employee priorities and questions | Let Team Member A add or reorder topics |
| 5 minutes | Progress and recognition | Review the five draft entries and checklist conflict identified |
| 8 minutes | Current work and dependencies | Confirm onboarding work and the IT security-access dependency |
| 7 minutes | Development | Discuss practicing part of the next onboarding session |
| 5 minutes | Decisions and actions | Confirm owners, dates, and next follow-up |

### Example action register

| Action | Owner | Due date | Dependency | Status | Confirmation needed |
|---|---|---|---|---|---|
| Review five service-request entries | Manager | September 23 | Policy-owner confirmation | Open | Confirm review date |
| Confirm security-access procedure | Manager | Needs confirmation | IT response | Blocked | Confirm IT owner and due date |
| Select onboarding section for practice | Team Member A and manager | Before next session | Session agenda | Proposed | Confirm section and coaching time |

The example does not rate the employee. It documents confirmed work, support, and decisions that still need clarification.

## Review guidance

Before sharing or storing any output:

1. Compare the draft with the original approved goals and notes.
2. Give the employee a reasonable way to correct factual errors.
3. Confirm owners and dates directly with the people involved.
4. Remove manager-only, private, or irrelevant information from the employee recap.
5. Move policy, complaint, accommodation, leave, safety, investigation, or employee-relations matters into the organization’s approved process.
6. Follow company rules for record retention, access, monitoring, transcripts, and AI use.
7. Keep the conversation human: ask, listen, clarify, and use judgment.

## Responsible-AI and privacy safeguards

- Use role-related information, not protected characteristics.
- Remove names and unnecessary identifiers where practical.
- Do not include medical, accommodation, leave, compensation, investigation, immigration, or employee-relations details in an external AI system.
- Do not record or upload meetings without required policy approval, notice, consent, and security controls.
- Do not use sentiment analysis, emotion recognition, personality scoring, or “culture fit” scoring.
- Do not infer agreement, intent, motivation, loyalty, potential, or future performance.
- Do not convert meeting frequency, note volume, or action counts into a performance score.
- Keep official decisions and documentation in approved systems with appropriate access controls.
- Use an employer-approved AI system when company information is involved.
- Require manager and employee verification of the factual recap.
- Keep qualified HR and leaders accountable for employment decisions.

## Intended impact

This workflow is designed to reduce meeting-preparation and note-organization time, make commitments easier to track, and improve clarity between managers and employees. Actual time savings and employee-experience results should be measured before making performance claims.

## Disclaimer

This resource provides general organizational support. It is not legal, employee-relations, investigation, accommodation, medical, or performance-management advice. Organizations should adapt it to approved policies and have qualified HR, privacy, security, and legal professionals review its use.

All people, roles, organizations, dates, and examples are fictional.
