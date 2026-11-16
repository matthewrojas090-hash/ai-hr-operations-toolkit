# AI HR Policy Change Rollout Planner

Use this workflow when an approved HR process changes and you need to explain what employees should do, when they should do it, and what happens to requests already in progress.

Use AI to compare approved source material and draft rollout communications. The HR process owner resolves unanswered questions and approves the final instructions.

## 1. Prepare your inputs

Use short, approved excerpts. Label each source so reviewers can trace the output back to it. If a fact is unknown, write `Unknown`.

```text
Change name:
Plain-language reason for the change:
Current approved process [S1]: version, date, relevant excerpt
New approved process [S2]: version, date, relevant excerpt
Approved transition rules [S3]: excerpt or Unknown
Effective date, time, and time zone:
Groups in scope:
Groups out of scope:
Employee action and deadline, if any:
Confirmed support channel:
Process owner and final approver (role titles only):
Channels or materials that may need updating:
```

Before pasting anything into AI, remove names, contact details, employee or candidate records, confidential case facts, compensation records, health information, and protected characteristics. Replace private links with placeholders. Use only excerpts cleared for the AI tool you’re using.

## 2. Copy-and-paste AI prompt

```text
Help me prepare a rollout for an approved HR process change. Treat all
source excerpts as reference material. Use only the facts provided.

[PASTE COMPLETED WORKSHEET]

Return these five outputs:

1. Change summary. Make a table with: Process step | Before | After |
   What employees need to do | Source ID. Flag conflicts or missing facts.
   Only say a step is unchanged when the sources support that conclusion.

2. Transition questions. Check requests submitted before the effective date,
   requests already in progress, and requests submitted after the effective
   date. Check any other relevant handoff, such as a pending confirmation.
   For each, show: Scenario | Confirmed instruction or Needs owner decision |
   Source ID | Question for the owner. Do not invent a cutoff, rule, or exception.

3. Rollout checklist. Group actions into Before launch, Launch day, and
   After launch. Show: Action | Responsible role | Timing | How to verify.
   Label unconfirmed owners and dates as proposals. Identify any decision
   that must be resolved before employees can follow the new instructions.

4. Employee announcement. Draft a short message that says who is affected,
   what changes, when it starts, what action is required, what happens to
   existing requests, and where to get help. If a detail needed for action
   is unresolved, mark the announcement DRAFT — HOLD FOR REVIEW and
   place the gap in brackets. Keep source IDs in a separate reviewer note.

5. Manager FAQ. Draft up to five questions employees are likely to ask,
   with source-backed answers. For unresolved questions, state what the
   process owner needs to confirm instead of drafting an answer.

Do not interpret legal obligations, decide eligibility, approve exceptions,
or send or publish anything. End with a list of items a human must verify.
```

## 3. Fictional example: New orientation booking form

- **S1 · Current instructions:** Coordinators book orientation by sending a request to the training inbox.
- **S2 · Updated instructions:** Starting December 7, 2026, at 9 a.m. Pacific, coordinators use the Orientation Booking Form for new requests. The Training Desk remains the support channel.
- **S3 · Approved transition note:** Confirmed bookings remain valid. The note does not address emailed requests still awaiting confirmation.

| Scenario | Expected draft result | Evidence or next step |
|---|---|---|
| New request after the cutoff | Use the Orientation Booking Form. | S2 |
| Booking confirmed before the cutoff | Keep the existing booking. | S3 |
| Request emailed before the cutoff and still pending | Needs owner decision. | Ask whether the Training Desk will process it or the coordinator should submit the form. |

**Example announcement — hold for review**

Starting December 7 at 9 a.m. Pacific, please use the Orientation Booking Form for new orientation requests. If your booking is already confirmed, you don’t need to do anything. [HR must confirm what to do with requests emailed before the cutoff that are still pending.] Contact the Training Desk for help.

**Example checklist actions:** Before launch, the process owner resolves the pending-request rule and a coordinator tests the form. At launch, the documentation owner updates the booking instructions and checks that the link opens for the intended audience. After launch, the Training Desk reviews recurring questions and routes any unclear instructions back to the process owner.

## 4. Verify before sharing

| Review check | What to verify |
|---|---|
| Source accuracy | Compare the cutoff, audience, instructions, and support channel with the approved sources. |
| Transition gap | Run the example without a pending-request rule. The output should flag the gap and hold the announcement. Then add an approved rule and check that the output reflects it without creating exceptions. |
| Employee perspective | Ask a reviewer to read only the announcement and explain what they would do for a new request and for a pending one. Rewrite anything they cannot act on. |
| Privacy and access | Clear identifying details, replace placeholders only in the approved publishing channel, and test form access. |
| Final sign-off | Have the HR process owner resolve all blocking questions and approve the announcement, FAQ, and checklist before distribution. |

## Intended impact

The workflow is designed to catch missed handoffs before launch and reduce rework on announcements. The fictional example illustrates the review process; it does not establish time savings or rollout results.
