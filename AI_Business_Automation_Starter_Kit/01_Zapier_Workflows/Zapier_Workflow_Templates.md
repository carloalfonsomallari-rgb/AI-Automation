# Zapier Workflow Templates

This folder includes 10 beginner-friendly, import-ready automation workflows designed to accelerate lead management, customer follow-up, and sales pipeline updates.

## Workflow 1: Google Form → CRM → Gmail automation
- Trigger: New response in Google Forms
- Actions:
  1. Create new lead in HubSpot or Pipedrive
  2. Send a Gmail confirmation email to the contact
- Apps: Google Forms, HubSpot (or Pipedrive), Gmail
- Setup instructions:
  1. Create your Google Form with fields for name, email, phone, and inquiry.
  2. Connect Google Forms to Zapier and choose "New Response in Spreadsheet." 
  3. Connect HubSpot/Pipedrive and map the form fields to lead name, email, phone, and notes.
  4. Connect Gmail and build a confirmation email using personalization variables.
  5. Test the Zap and enable it.
- Workflow explanation: This automation captures inbound leads from a form, creates a contact record, and immediately sends a professional welcome message.

## Workflow 2: Lead capture → Google Sheets → HubSpot
- Trigger: New row in Google Sheets
- Actions:
  1. Create or update contact in HubSpot
  2. Add row to a second worksheet for lead scoring review
- Apps: Google Sheets, HubSpot
- Setup instructions:
  1. Build a Google Sheet with columns: Date, Name, Email, Phone, Source, Interest, Score.
  2. Connect Google Sheets to Zapier and choose "New Spreadsheet Row." 
  3. Map the row data to HubSpot contact fields.
  4. Add an action to append a row in a "Lead Review" sheet.
  5. Turn on Zap.
- Workflow explanation: Creates a clean lead entry in HubSpot while also building a manual review sheet for sales prioritization.

## Workflow 3: Missed call → automatic follow-up email
- Trigger: New call activity in RingCentral or CallRail marked as missed
- Actions:
  1. Create a new task in Asana or Trello
  2. Send a follow-up Gmail message to the missed caller
- Apps: RingCentral, CallRail, Gmail, Asana/Trello
- Setup instructions:
  1. Connect your call tracking service to Zapier.
  2. Filter the trigger for "missed call" only.
  3. Create a task in Asana/Trello assigned to your sales rep.
  4. Send a Gmail follow-up with a template such as: "Sorry we missed you — can we schedule a quick call today?"
- Workflow explanation: Ensures every missed inquiry becomes a fast follow-up opportunity rather than a lost lead.

## Workflow 4: Appointment booking → calendar confirmation
- Trigger: New appointment in Calendly or Acuity Scheduling
- Actions:
  1. Send confirmation email via Gmail
  2. Create event in Google Calendar with service details
- Apps: Calendly/Acuity, Gmail, Google Calendar
- Setup instructions:
  1. Authorize Calendly or Acuity in Zapier.
  2. Use "Invitee Created" as trigger.
  3. Build a confirmation email including appointment date, time, and next steps.
  4. Create a Google Calendar event with the invitee information.
- Workflow explanation: Automates appointment confirmations and calendar updates so bookings never slip through.

## Workflow 5: Website inquiry → CRM update
- Trigger: New form submission from Typeform, Jotform, or website contact page
- Actions:
  1. Find or create contact in Zoho CRM or HubSpot
  2. Update lead status to "New Inquiry"
  3. Push notes into a deal or contact record
- Apps: Typeform/Jotform, Zoho CRM/HubSpot
- Setup instructions:
  1. Connect your website form service.
  2. Add a lookup step to find existing contacts.
  3. Create or update the contact with inquiry details.
  4. Set the lead status field to "New Inquiry."
- Workflow explanation: Collects website leads and keeps CRM data fresh and actionable.

## Workflow 6: Facebook Lead Form → Email sequence
- Trigger: New lead from Facebook Lead Ads
- Actions:
  1. Add subscriber to ActiveCampaign or Mailchimp
  2. Send a welcome email or SMS via Twilio
- Apps: Facebook Lead Ads, ActiveCampaign/Mailchimp, Twilio
- Setup instructions:
  1. Connect Facebook Lead Ads and choose your lead form.
  2. Map lead fields to your email marketing provider.
  3. Create a welcome email or SMS message.
  4. Activate the Zap.
- Workflow explanation: Turns social media leads into engaged prospects automatically.

## Workflow 7: Lead qualification workflow
- Trigger: New lead added to CRM with a "New" status
- Actions:
  1. Send a short qualification survey via Gmail
  2. Add a note in CRM with survey link and lead source
- Apps: HubSpot/Pipedrive, Gmail
- Setup instructions:
  1. Use CRM event trigger on new contact or deal creation.
  2. Send an automated email with a qualification survey link.
  3. Update the contact note with lead details.
- Workflow explanation: Automates the first qualification step so high-value leads are identified quickly.

## Workflow 8: Customer onboarding workflow
- Trigger: New customer deal closed in CRM
- Actions:
  1. Add customer to onboarding board in Trello or Asana
  2. Send a welcome packet email
  3. Create a recurring follow-up task after 7 days
- Apps: HubSpot, Trello/Asana, Gmail
- Setup instructions:
  1. Trigger on deal stage changed to "Won" or "Client." 
  2. Create board card or task with onboarding checklist.
  3. Send a welcome email with links to next steps.
  4. Schedule a follow-up task.
- Workflow explanation: Creates a consistent onboarding path for every new client.

## Workflow 9: Client follow-up automation
- Trigger: Completed service appointment or delivered project milestone
- Actions:
  1. Add client to follow-up list in Google Sheets
  2. Send personalized thank-you email with next steps
- Apps: Google Sheets, Gmail, Google Calendar
- Setup instructions:
  1. Use a completed event trigger or spreadsheet row addition.
  2. Log client details into follow-up sheet.
  3. Send a thank-you email with a link to schedule the next appointment.
- Workflow explanation: Encourages repeat business by keeping clients in a follow-up cadence.

## Workflow 10: Sales pipeline update automation
- Trigger: Deal stage changes in CRM
- Actions:
  1. Notify sales leader in Slack or Microsoft Teams
  2. Add internal note with next action and due date
- Apps: HubSpot/Pipedrive, Slack/Teams
- Setup instructions:
  1. Connect your CRM and choose a deal stage update trigger.
  2. Send a message to the sales channel with deal name, value, and next step.
  3. Update the CRM note field.
- Workflow explanation: Keeps the team aligned on pipeline movement and ensures next actions are tracked.
