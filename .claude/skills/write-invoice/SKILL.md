---
name: write-invoice
description: Use this skill when someone asks to generate an invoice, create a bill, write a payment receipt, produce a delivery invoice, or calculate charges for a customer delivery
allowed-tools:
  - read_file
  - write_file
---

## Generating a LagosDeliver Invoice

When this skill is activated:

1. Ask for these details if not provided:
   - Customer full name and address
   - Tracking number (format: LD-XXXXX)
   - Type of delivery (Standard or Express)
   - Pickup location (city)
   - Delivery location (city)
   - Package weight in kg
   - Date of delivery

2. Read formatting.md for detailed formatting rules

3. Read templates.md and select the correct template:
   - Use STANDARD template for standard deliveries
   - Use EXPRESS template for express deliveries

4. Calculate the charges:
   - Standard base fee: ₦1,500
   - Express base fee: ₦3,500
   - Weight surcharge: ₦200 per kg above 5kg
   - Interstate surcharge: ₦500 (if different states)

5. Generate the invoice using the selected template

6. Save the invoice as: invoice-LD-XXXXX.md

7. Confirm to the user that the invoice has been generated
   and tell them the filename

## Important Rules
- Always double-check all calculations before presenting
- Never leave any field blank — use N/A if unknown
- Always include the invoice generation date and time
- VAT is 7.5% — always calculate and include it