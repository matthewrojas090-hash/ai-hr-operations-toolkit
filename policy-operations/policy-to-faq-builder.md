# AI Policy-to-FAQ Builder

Turn an approved workplace policy into a clear, source-linked FAQ that HR can review before sharing.

## What this tool does

Employees often ask the same policy questions in different ways. HR may spend time finding the correct section, translating formal wording, and checking whether an answer is still current.

This workflow helps HR teams:

- Draft plain-language answers from an approved policy
- Link every answer to a specific policy section
- Identify questions the policy does not answer
- Separate policy facts from suggested next steps
- Route exceptions and sensitive questions to the right human owner
- Create consistent employee-facing guidance
- Flag wording that may be outdated or unclear

AI drafts the FAQ. An authorized HR or policy owner verifies and approves it before anyone relies on it.

## When to use it

Use this workflow for current, approved workplace procedures such as equipment requests, office access, expense submission, or routine onboarding steps.

Do not use it to decide an individual employee's eligibility, interpret a disputed policy, resolve an employee-relations matter, or give legal advice. Send those questions through the organization's approved process.

## What you need

Prepare:

1. The current approved policy or procedure
2. Its title, version, effective date, and owner
3. The audience allowed to receive the FAQ
4. Any approved request or escalation route
5. Common questions with all employee details removed

Use an employer-approved AI system for internal material. Do not paste employee records, health information, accommodation requests, investigation details, compensation records, or confidential case notes.

## Input template

```text
POLICY DETAILS

Policy title:
Version or approval date:
Effective date:
Policy owner:
Approved audience:
Source location or document identifier:
Is this the current approved version? Yes / No / Unknown

APPROVED SOURCE TEXT

[PASTE THE RELEVANT APPROVED POLICY TEXT, WITH SECTION NUMBERS]

COMMON QUESTIONS

[List de-identified questions. Do not include individual cases.]

ROUTING

Approved request channel:
Approved escalation owner:
Topics that must always go to a person:
Known exceptions requiring human review:
```

If the current version cannot be confirmed, stop before publishing an FAQ.

## Copy-and-paste AI prompt

```text
You are helping an HR team draft an employee-facing FAQ from an approved policy.

Use only the policy text and routing information supplied below. Do not invent rules, eligibility, deadlines, exceptions, legal requirements, approvals, contact details, or company practices.

Treat common questions as questions, not as evidence of what the policy says.

Source material:
[PASTE THE COMPLETED INPUT TEMPLATE]

Produce the following:

1. Source check

State the policy title, version, effective date, owner, and approved audience exactly as supplied. Flag any missing or conflicting metadata. If the source is not confirmed as current and approved, label the entire output "Draft — do not publish."

2. FAQ

Draft up to 12 common questions and answers in plain language.

Use this table:

| Question | Draft answer | Source section | What remains unclear | Review owner |
|---|---|---|---|---|

Rules:
- Every factual answer must cite the relevant section number or exact heading from the supplied policy.
- If a question is not answered by the policy, write "The supplied policy does not answer this question."
- Do not infer an exception from an example.
- Do not turn a recommendation into a requirement.
- Do not make a promise about an individual's outcome.
- Keep answers short enough for an employee to understand on first read.

3. Action steps

For questions with a documented process, list the steps in the order given by the source. Name an owner or channel only when supplied. Flag missing owners and deadlines.

4. Human-review queue

List:
- Unanswered questions
- Ambiguous or conflicting policy language
- Questions involving exceptions
- Questions that require an individual determination
- Statements that may need privacy, security, HR, or legal review

Give each item an owner if one was provided. Otherwise write "Owner needs confirmation."

5. Employee-facing introduction

Write a short introduction explaining the FAQ's topic, policy version, and where employees should go for questions. Do not imply that the FAQ replaces the approved policy.

6. Publication checklist

Create a checklist for the policy owner to confirm:
- The source version is current
- Every answer matches its cited section
- No answer invents an exception or deadline
- Links and channels work
- The audience is correct
- Private information has been removed
- Unanswered questions have been routed
- An authorized person approved the FAQ

Finish with this statement:
"This FAQ is a draft based on the supplied source. The policy owner must verify it against the current approved policy before publication."
```

## Fictional example

### Approved source excerpt

```text
Policy: Northstar Labs Visitor Access Procedure
Version: 2.0
Effective date: September 1
Owner: Workplace Operations
Approved audience: Employees
Current approved version: Yes

Section 1 — Request
An employee expecting a visitor submits a visitor request through the
workplace portal at least one business day before the visit.

Section 2 — Arrival
Visitors check in at reception and receive a temporary badge.

Section 3 — Onsite responsibility
The hosting employee meets the visitor at reception and remains responsible
for escorting the visitor in restricted areas.

Approved request channel: Workplace portal
Approved escalation owner: Workplace Operations
```

### Example FAQ output

| Question | Draft answer | Source section | What remains unclear | Review owner |
|---|---|---|---|---|
| How do I request a visitor? | Submit a visitor request through the workplace portal at least one business day before the visit. | Section 1 — Request | None in the supplied text | Workplace Operations |
| Where does my visitor check in? | At reception, where they will receive a temporary badge. | Section 2 — Arrival | None in the supplied text | Workplace Operations |
| Can I bring a visitor without advance notice? | The supplied policy does not answer this question. Contact Workplace Operations for guidance. | No supporting section | Whether an exception exists | Workplace Operations |

The example does not invent a same-day exception.

All organizations, policies, and details in this example are fictional.

## HR review before publication

The policy owner should compare each answer with the current source document, confirm that the cited section supports it, check the request channel, and resolve unanswered questions.

Review the FAQ again whenever the policy changes. Record the FAQ review date and source version so readers can tell which policy it reflects.

## Responsible AI and privacy

- Use only current, approved policy material.
- Remove individual employee questions and case details.
- Do not include health, accommodation, investigation, compensation, or other sensitive records.
- Never ask AI to decide an individual's eligibility or exception.
- Do not present an AI interpretation as an official policy decision.
- Route ambiguous or sensitive matters to qualified people.
- Keep a human policy owner accountable for publication and updates.

## Intended impact

This workflow is designed to reduce repeated policy lookups and make routine HR answers clearer and more consistent. Measure any time savings or service improvements before claiming a result.

## Disclaimer

This is an organizational drafting aid, not legal advice or an official policy. Each organization must review the output against its own current, approved materials.
