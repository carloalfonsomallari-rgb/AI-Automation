# CRM Automation System

A beginner-friendly CRM automation system designed to track leads, manage pipeline stages, trigger follow-ups, and keep a status dashboard visible.

## CRM Fields

Use these fields in HubSpot, Pipedrive, Zoho, or your preferred CRM.

- Lead Name
- Company Name
- Email Address
- Phone Number
- Lead Source
- Industry
- Service Interest
- Lead Score
- Status (New, Contacted, Qualified, Proposal, Negotiation, Closed Won, Closed Lost)
- Next Action
- Next Action Date
- Follow-up Reminder
- Priority
- Notes
- Deal Value
- Expected Close Date

## Lead Tracker

Build a lead tracker view with these columns:

- Date Added
- Name
- Email
- Phone
- Source
- Interest Level
- Lead Score
- Status
- Next Action
- Next Action Date
- Assigned To
- Notes

### Lead scoring logic

- Website inquiry = 10 points
- Referral = 15 points
- High-value service interest = 20 points
- Responded to first email = 10 points
- Booked appointment = 25 points
- Requested proposal = 30 points

Use a formula field or sheet to calculate the total score.

## Sales Pipeline

Create these stages in your CRM pipeline:

1. New Inquiry
2. Contacted
3. Qualified
4. Proposal Sent
5. Negotiation
6. Decision Pending
7. Closed Won
8. Closed Lost

Each stage should have a clear next action note and follow-up date.

## Follow-up Reminder System

Use automated tasks or reminders that trigger when:

- Status changes to Contacted → follow up in 2 days
- Status changes to Qualified → send proposal within 24 hours
- Status changes to Proposal Sent → check in after 3 days
- Status changes to Negotiation → follow up every 5 days
- Lead Score exceeds 50 → assign to senior rep

### Example automation rules

1. If Lead Score ≥ 50 and Status = New, assign to "High Value Lead" queue and send Slack notification.
2. If Next Action Date is today, create a task and email reminder to the owner.
3. If status remains "Contacted" for more than 5 days, update to "Stale" and trigger a re-engagement sequence.

## Status Tracker

Build a dashboard using the CRM reporting feature or Google Sheets/Airtable with these widgets:

- New leads this week
- Qualified leads this week
- Proposals sent today
- Deals won this month
- Deals lost and reason breakdown
- Lead score distribution
- Follow-up overdue count
- Top 5 lead sources

## Dashboard Structure

Example dashboard sections:

### 1. Pipeline Health
- Active deals by stage
- Value by stage
- Conversion rate from Qualified to Proposal

### 2. Lead Intake
- New leads by source
- Top service interest categories
- Lead score average

### 3. Follow-up Performance
- Overdue follow-ups
- Completed actions this week
- Response time average

### 4. Revenue Forecast
- Expected close date timeline
- Weekly deal velocity
- Estimated monthly revenue

## Implementation notes

- Use consistent naming across your CRM and marketing tools.
- Keep the "Next Action" field updated on every lead change.
- Review the dashboard each morning to identify hot leads and overdue tasks.
- Customize scoring weights for your specific business model.
- Use automation tools like Zapier/Make to move leads through stages and trigger reminders.
