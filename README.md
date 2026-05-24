# Automated Client Billing System

An n8n workflow that automatically generates and emails 
PDF invoices to clients on a monthly schedule.

## What it does
- Reads unbilled line items from Google Sheets
- Groups by client and calculates totals
- Generates professional PDF invoices via PDFBolt
- Emails each client their invoice via Gmail
- Marks rows as Billed in Google Sheets

## Tech stack
n8n · Google Sheets · PDFBolt · Gmail API · JavaScript
