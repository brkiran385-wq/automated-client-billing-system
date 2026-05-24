# Automated Finance Operations Suite

Two production-grade n8n automation workflows built 
to eliminate manual finance admin tasks.

---

## Project 1 — Automated Client Billing System

![Invoice Workflow] <img width="1262" height="608" alt="Screenshot 2026-05-24 at 11 07 36 PM" src="https://github.com/user-attachments/assets/cf9f0087-7768-432b-b7e6-d3791986609f" />


An event-driven pipeline that automatically generates 
and distributes PDF invoices to 15 clients monthly.

### What it does
- Reads unbilled line items from Google Sheets
- Groups by client and calculates totals dynamically
- Generates professional PDF invoices via PDFBolt
- Emails each client their invoice via Gmail
- Marks rows as Billed to prevent duplicate invoicing

### Tech stack
n8n · Google Sheets · PDFBolt · Gmail API · JavaScript

---

## Project 2 — Financial Health Monitor

![Health Monitor Workflow] <img width="1261" height="646" alt="Screenshot 2026-05-24 at 11 05 45 PM" src="https://github.com/user-attachments/assets/dafae69f-6929-44a4-b004-b0ea895a8b12" />

A weekly automated pipeline that monitors financial 
health indicators across 10 client accounts and alerts 
relationship managers to at-risk clients.

### What it does
- Reads weekly financial data from Google Sheets
- Computes current ratio, debtor days, gross margin, 
  cash runway per client
- Flags Critical and Watch clients automatically
- Generates plain-English advisory notes per client
- Emails urgent alerts every Monday at 8am

### Tech stack
n8n · Google Sheets · Gmail API · JavaScript

---

## Problem Statement

Service-based businesses and finance departments lack 
automated systems to track billing cycles and monitor 
client financial health — resulting in delayed revenue 
recognition, missed distress signals, and significant 
non-billable admin hours. These workflows eliminate 
that gap entirely.

## How to use
1. Import either `.json` file into your n8n instance
2. Connect Google Sheets and Gmail credentials
3. Point to your own dataset
4. Activate — runs automatically on schedule
