# Siddaganga College Admission Portal

Static college portal concept with an admission enquiry form connected to an n8n webhook.

## Files
- `index.html` — complete website with responsive design and admission form.
- `siddaganga_admission_automation.json` — starter n8n workflow.

## Webhook
The form is configured to POST submissions to:
`https://dhyan07.app.n8n.cloud/webhook/siddaganga-admission-enquiry`

Ensure the matching n8n workflow is active and its Google Sheets and Gmail credentials are configured before accepting real enquiries.

## Google Sheets headers
Enquiry ID, Submitted At, Full Name, Email Address, Phone Number, Programme, Qualification, Admission Year, Message, Enquiry Status, Email Status

## Important
The form sends data to the configured webhook. Successful recording and email delivery depend on the n8n workflow being correctly configured and active. Test with sample data before sharing the site publicly. The webhook URL is visible in the public website source; add suitable spam protection and rate limiting before production use. Verify college details and privacy/consent requirements before official use.
