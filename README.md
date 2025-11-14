# n8n_invoice_reminder
A smart invoice reminder automation tool featuring a user-friendly dashboard connected with n8n workflows via webhooks. It automatically checks for unpaid invoices and sends reminder notifications, while allowing users to mark invoices as paid directly through the dashboard.

How It Works:
The automation checks a Google Sheet where all invoices are listed.
The workflow runs on a regular schedule and looks for invoices that are still unpaid.
Depending on the situation, it sends a different type of email:
1. First Reminder
Sent when the invoice is unpaid and no previous reminder was sent.
2. Follow-Up Reminder
Sent if the invoice is still unpaid after the first reminder.
3. Late Payment Reminder
Sent when the invoice has passed the due date.
Each email has a different tone and message style so communication feels natural rather than repetitive.

Dashboard (Lovable):
To make the system easy to use, I created a small dashboard where the user can:
View all invoices in one place
See which ones are unpaid
Send reminders manually (optional)
Update the status from Unpaid → Paid with one click
When the status is changed to “Paid,” the workflow automatically updates in google sheet and will stop sending reminders for that invoice.

Tech Stack:
n8n – for automation logic
Google Sheets – as the invoice database
Lovable – for the dashboard and UI
Email (SMTP / Gmail) – for sending reminders

Future Improvements:
Some possible upgrades I may add later:
SMS reminders
Integration with Stripe or PayPal
Auto-generated PDF invoices
Client portal for viewing paid/unpaid invoices



<img width="1813" height="725" alt="Screenshot 2025-11-14 151117" src="https://github.com/user-attachments/assets/5810d5d0-4b7a-40a0-b18e-dbfc9a8f664a" />
<img width="1680" height="868" alt="Screenshot 2025-11-14 150211" src="https://github.com/user-attachments/assets/b49fa86e-e258-412e-930b-bc80271c00d9" />
