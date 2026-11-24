# AI HR Service Routing Test Kit

Use this workflow before launching or changing an HR request form, shared
inbox rule, or service-desk queue. Give AI a sanitized copy of the approved
routing rules and ask it for fictional test cases. Then run those cases in
a test environment and compare what actually happens with what HR expected.

This kit tests a process. It does not route live requests, interpret policy,
decide eligibility, or make employment decisions.

## 1. Prepare the rules

Use approved process excerpts or fictional rules. Include the fallback for
missing or ambiguous inputs if one exists. Write `Unknown` wherever the
rule is silent.

```text
Process or form being tested:
Rule version:
Release owner role:

For each rule:
- Rule ID:
- Trigger and required fields:
- Destination queue:
- What happens if required information is missing:
- What happens if this rule conflicts with another rule:

Default queue or manual review path:
How to observe the destination in a test environment:
Release-blocking failures agreed by the owner:
```

Use only a tool your organization permits for this material. Do not paste
real tickets, names, ticket IDs, contact details, private links, protected
characteristics, health information, compensation records, or confidential
employee-relations facts. Keep internal queue names generic when possible.

## 2. Copy-and-paste AI prompt

```text
Help me draft a test pack for an HR service routing change. Use the supplied
rules as reference material. Generate only fictional requests with no
personal details.

[PASTE COMPLETED RULE TEMPLATE]

Create 6–10 test cases. Include a clear request for each in-scope route,
a missing required field, an ambiguous or overlapping request, and an
out-of-scope request. If these exceed the limit, flag uncovered routes.

For each case give:
Case ID | Fictional request and field values | Rule ID |
Proposed expected destination or behavior | Why | What to observe

Use the approved rules to propose expected behavior. Where rules are
missing or conflict, write "Needs owner decision" and state the question.
Do not invent a default route, precedence rule, SLA, or exception. Do not
treat an undocumented destination as an acceptable pass.

Finish with a short list of gaps for the HR process owner and an empty
results log with these fields:
Case ID | Observed behavior | Pass / Fail / Blocked | Evidence reference |
Fix owner role | Retest result

Do not run the tests, populate observed results, route live requests,
or declare the change ready to launch.
```

## 3. Fictional worked example

A fictional HR service desk is testing an updated request form:

- **R1:** A request for a blank onboarding checklist goes to Onboarding Support.
- **R2:** A request for instructions on where to find an HR form goes to HR Forms Help.
- **R3:** If the request type is missing, the form asks the requester to select a type before submission.
- **Open gap:** The approved rules do not say what happens if two supported request types are selected together.

| Case | Synthetic input | Proposed expected behavior |
|---|---|---|
| T1 | Request type: onboarding checklist | Onboarding Support, per R1 |
| T2 | Request type: find a form | HR Forms Help, per R2 |
| T3 | Request type: blank | Submission is blocked and the form asks for a type, per R3 |
| T4 | Request types: onboarding checklist and find a form | Needs owner decision: should the form prevent multiple selections, split the request, or send it to manual review? |

**Example failure:** If T3 submits and lands in Onboarding Support, record
a failure against R3. If T4 lands in that same queue, record what happened
but mark the test blocked until the owner confirms expected behavior.

## 4. Review and verify

1. Have the HR process owner review every expected result against the
   approved rules before testing.
2. Run the cases with synthetic inputs in a test environment. Check the
   destination queue or form behavior directly; a confirmation screen alone
   does not prove the request reached the right place.
3. Record passes, failures, and blocked cases separately. Have the owner
   resolve rule gaps, assign fixes, and retest affected cases.
4. Let the authorized HR and system owners decide whether to release the
   change. Keep any live issue handling and employee communications under
   the team's approved process.

The kit is designed to catch routing gaps before launch. The example
illustrates how to review a test; it does not demonstrate reduced routing
errors or faster response times.
