---
name: customer-email
description: Use this skill when someone asks to write a customer email, draft an email to a client, compose a delivery notification, send a message to a customer, write a delay apology email, or write any business communication related to LagosDeliver deliveries
allowed-tools:
  - read_file
  - write_file
model: claude-sonnet-4-20250514
---

## Writing a Customer Email for LagosDeliver

When this skill is activated:

1. Ask for these details if not provided:
   - Customer's full name
   - Type of email needed:
     * Delivery confirmation
     * Delivery delay apology
     * Package not found
     * General enquiry response
     * Invoice/payment email
   - Tracking number (if relevant)
   - Any specific details to include

2. Write the email in this format:

---

**Subject:** [Clear, specific subject line]

Dear [Customer Name],

[Opening — warm and professional greeting]

[Main body — clear explanation of the situation]

[Action required or next steps — be specific]

[Closing — positive and helpful]

Warm regards,
LagosDeliver Customer Service Team
support@lagosdeliver.com
0800-LAGOS-DLV

---

3. Rules for every email:
   - Always address customer by name
   - Never blame the customer
   - If there is a problem, apologize first before explaining
   - Always include tracking number when relevant
   - Always give a specific next step or action
   - Keep it under 200 words unless absolutely necessary
   - Use warm Nigerian professional English

4. Email templates by type:

### Delivery Confirmation
Subject: Your Package LD-XXXXX Has Been Delivered! 🎉

### Delay Apology
Subject: Important Update About Your Delivery LD-XXXXX

### Package Not Found
Subject: We Need Your Help — Package LD-XXXXX

### General Response
Subject: Re: Your Enquiry — LagosDeliver Support