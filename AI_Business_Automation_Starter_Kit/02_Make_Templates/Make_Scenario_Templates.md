# Make.com Scenario Templates

This guide contains 10 automation templates for Make.com (Integromat) with scenario structure, module connections, logic explanation, and setup guidance.

## Scenario 1: New lead form → CRM lead record → Slack alert
- Modules:
  1. Webhooks > Custom webhook (form submission)
  2. CRM > Create or update contact
  3. Slack > Send message
- Logic:
  - Incoming form submissions trigger the scenario.
  - The system checks for an existing contact.
  - If no match exists, it creates the lead and sends an internal alert.
- Setup guide:
  1. Create a webhook in Make and paste the URL into your lead form handler.
  2. Map name, email, phone, and inquiry details to CRM fields.
  3. Add a Slack message module with a summary and urgency tag.

## Scenario 2: SMS reminder for missed appointments
- Modules:
  1. Google Calendar > Watch events
  2. Filter > Event status is canceled or no-show
  3. Twilio > Send SMS
- Logic:
  - Watch calendar appointments.
  - When a booked event is canceled or shows as missed, send an SMS reminder with reschedule instructions.
- Setup guide:
  1. Connect Google Calendar and select the appointment calendar.
  2. Add a filter for event changes.
  3. Authorize Twilio and create a text message template.

## Scenario 3: New Facebook Lead → Google Sheet + Email nurture
- Modules:
  1. Facebook Lead Ads > Watch leads
  2. Google Sheets > Add row
  3. Gmail > Send email
- Logic:
  - Capture lead details from Facebook.
  - Log the lead in a spreadsheet.
  - Immediately send a welcome email with next-step instructions.
- Setup guide:
  1. Connect Facebook Lead Ads to monitor your form.
  2. Create a Google Sheet with headers for name, email, source, and notes.
  3. Build an email template in Gmail.

## Scenario 4: New CRM deal → contract generation → email delivery
- Modules:
  1. CRM > Watch new deals
  2. PDF generator > Create contract from template
  3. Gmail > Send contract email
- Logic:
  - When a new deal enters the "Proposal" or "Contract" stage, automatically generate a PDF contract and email it to the prospect.
- Setup guide:
  1. Connect your CRM and specify the deal stage.
  2. Create a contract template with dynamic fields.
  3. Send the PDF via Gmail to the lead.

## Scenario 5: Lead score update → priority list → Zapier handoff
- Modules:
  1. Google Sheets > Watch rows
  2. Tools > Iterator
  3. HTTP > Webhook (Zapier)
- Logic:
  - Review a lead spreadsheet for updated score values.
  - Identify high-priority leads.
  - Trigger a Zapier webhook for urgent follow-up actions.
- Setup guide:
  1. Maintain a Google Sheet with lead scoring formulas.
  2. Use the Iterator module to process each changed row.
  3. Set up a Zapier webhook URL to receive high-priority lead alerts.

## Scenario 6: New invoice paid → client onboarding checklist
- Modules:
  1. QuickBooks Online/Xero > Watch payments
  2. Google Workspace > Create document
  3. Google Drive > Upload file
- Logic:
  - When client payment is received, generate an onboarding checklist document and save it for the team.
- Setup guide:
  1. Authorize your accounting app and select incoming payments.
  2. Build a document template with client name, project, and next steps.
  3. Save the file in your shared drive folder.

## Scenario 7: New review or testimonial → social media queue
- Modules:
  1. Email > Watch emails
  2. Text parser > Extract testimonial text
  3. Airtable/Google Sheets > Add row
- Logic:
  - Monitor feedback emails or form submissions.
  - Extract positive review content.
  - Queue it for your social media or marketing team.
- Setup guide:
  1. Create an email filter for feedback submissions.
  2. Use the text parser to capture the testimonial.
  3. Save it to an approval queue sheet.

## Scenario 8: Client milestone reached → reward email + Slack update
- Modules:
  1. CRM > Watch deal stage
  2. Email > Send congratulation
  3. Slack > Send message
- Logic:
  - When a client moves to a milestone stage, send a congratulatory email and notify the team.
- Setup guide:
  1. Connect your CRM stage updates.
  2. Use an email module to send the milestone message.
  3. Send a Slack message to the project owner.

## Scenario 9: New proposal request → automated quote draft
- Modules:
  1. Webhooks > Custom webhook
  2. Google Docs > Create document from template
  3. Email > Send document link
- Logic:
  - Incoming proposal requests create a quote draft document automatically.
- Setup guide:
  1. Create a webhook for proposal intake forms.
  2. Build a quote template in Google Docs.
  3. Send the draft link to the requester for review.

## Scenario 10: Weekly pipeline summary → executive report
- Modules:
  1. Google Sheets/Airtable > Search records
  2. Iterator > Collect key metrics
  3. Gmail > Send summary email
- Logic:
  - Pull weekly pipeline data and send a concise report to leadership.
- Setup guide:
  1. Maintain a spreadsheet or base with pipeline stages.
  2. Use Iterator to calculate totals and conversion rates.
  3. Deliver the report via email.
