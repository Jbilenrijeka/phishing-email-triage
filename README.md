# Phishing Email Triage

A Junior SOC Analyst portfolio exercise demonstrating the initial assessment of a fictional suspicious email.

## Investigation Summary

The sample threatens account suspension within 30 minutes and asks the recipient to confirm a password through a link. Additional observations include a generic greeting and different From and Reply-To addresses.

**Initial disposition:** Suspicious; escalate for validation.

The request is consistent with a potential credential-harvesting attempt. However, the destination page was not examined, and no credential submission or account compromise is established.

## Scope and Evidence

This exercise uses a fictional plain-text email. The assessment is limited to the fields and message body included in the sample.

- The link uses a reserved `.invalid` domain.
- No live domain reputation checks were performed.
- No SPF, DKIM, or DMARC results are available.
- No attachment or payload is present.
- Delivery to real users and user interaction are not established.

## Analysis Workflow

1. Review the sender, Reply-To address, subject, and message body.
2. Identify urgency, password requests, and other suspicious indicators.
3. Assess each observation alongside its limitations.
4. Record an initial disposition and recommended validation steps.

## Skills Demonstrated

- Initial phishing email triage.
- Review of visible sender and Reply-To fields.
- Recognition of social engineering indicators.
- Evidence-based assessment with explicit limitations.
- Clear investigation documentation and escalation recommendations.

## Repository Files

| File | Contents |
| --- | --- |
| [sample_email.txt](sample_email.txt) | Fictional email used in the exercise. |
| [triage_report.md](triage_report.md) | Findings, evidence assessment, limitations, and recommended next steps. |

## Recommended Follow-Up in a Real Environment

These actions are recommendations and were not performed in this exercise:

- Preserve the original email and full headers.
- Review authentication results and mail gateway verdicts.
- Search for related messages and identify recipients.
- Determine whether anyone clicked the link or submitted credentials.
- Apply containment measures according to organizational policy and validated findings.

## Safety

Analyze real suspicious messages only through approved procedures. Do not open suspicious links or attachments directly on a personal or production device.
