# Workflow automation brief — representative portfolio sample

Prepared by Frenz Carl Asibuque. Fictional workflow; not a deployed client integration.

## Goal
Turn a website enquiry into a structured record and an assigned follow-up task without losing submissions.

## Trigger and data
- Trigger: a validated enquiry form is submitted.
- Required fields: name, email, enquiry type, request summary.
- Optional fields: preferred timeline and existing tools.
- Add submission ID and timestamp at intake.
- Do not collect passwords or unnecessary personal information.

## Proposed actions
1. Validate required fields and flag invalid records.
2. Check the submission ID to avoid creating duplicate tasks on retries.
3. Store the structured record in the agreed destination.
4. Route the task according to enquiry type.
5. Notify the assigned owner through the team's approved channel.
6. Record status and any failure for follow-up.

## Optional AI step
Summarize a long enquiry into a short internal brief. Preserve the original text and mark the summary as AI-assisted. Do not let the summary invent requirements or make promises to the enquirer. The owner reviews it before use.

## Exceptions
- Invalid email: retain as a review item; do not send an acknowledgement blindly.
- Unknown enquiry type: send to a default review queue.
- API failure: retry according to agreed rules and retain an error log.
- Duplicate submission: update or ignore according to the defined policy.
- Automation cannot choose a priority from sensitive personal characteristics.

## Platform selection
Choose the integration platform after checking connector availability, credentials, rate limits, error handling, and the client's existing subscriptions. This brief does not establish that any third-party integration is already live.

## Acceptance checks
- Valid submission creates one record and one task.
- Repeated delivery of the same submission does not create duplicates.
- Missing fields produce an actionable review item.
- Service failures remain visible to the owner.
- AI output is reviewable alongside the original input.
- Ownership, access, and maintenance responsibilities are documented.
