---
name: track-shipment
description: Use this skill when someone asks to track a package, check delivery status, find a shipment, or locate an order using a tracking number
allowed-tools:
  - read_file
  - write_file
---

## Tracking a LagosDeliver Shipment

When this skill is activated:

1. Ask for the tracking number if not provided
   - Format must be: LD-XXXXX (example: LD-12345)
   - If wrong format, politely ask them to check again

2. Confirm the tracking number with the customer

3. Provide a status update in this format:

## Shipment Status Report

**Tracking Number:** LD-XXXXX  
**Status:** In Transit / Delivered / Pending  
**Origin:** [City]  
**Destination:** [City]  
**Estimated Delivery:** DD/MM/YYYY  
**Last Location:** [Most recent location]  

## Delivery Timeline
- [Date] — Package picked up from sender
- [Date] — Arrived at Lagos hub
- [Date] — Out for delivery
- [Date] — Delivered ✅

4. If package is delayed, apologize and give new estimate
5. Always end by asking if customer needs anything else