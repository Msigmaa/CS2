# Load It Up

## Changelog
**[v1.0] — 2025-08-15**
- Initial specification and README completed
- Defined problem, objectives, inputs/outputs, and logic plan
- Ready for project development

---

## Project
**Load It Up** — a lightweight personal expense logger that queues and syncs transactions when LOAD/WIFI is available.

---

## Overview
Load It Up is a mobile-friendly tool designed for individuals who primarily spend on prepaid load, data promos, subscriptions, and other small, frequent transactions.  
It works offline by queuing entries and automatically syncing them once an internet connection is detected.

---

## Problem Statement
Many people overspend on small, frequent purchases like load and data promos because they fail to track them.  
Load It Up helps users record these transactions, visualize spending habits, and manage budgets effectively.

---

## Objectives
- Log and categorize expenses and income  
- Track spending patterns with charts  
- Set and monitor savings goals  
- Provide monthly expense summaries  

---

## Features
- Manual entry for expenses and income  
- Categories: Load, Data/WiFi, Bills, Subscriptions, Personal  
- Offline queue with automatic sync when online  
- Monthly summary and category pie chart  
- Savings goal progress tracking  

---

## Inputs
- Amount  
- Category  
- Date/time (auto or manual)  
- Optional note  

---

## Outputs
- Running balance  
- Category totals per month  
- Savings goal progress bar  
- Monthly report in PDF or CSV  

---

## Logic Plan (Pseudocode)


START
LOAD local_db
IF first_run THEN create_profile(), set_saving_goal()
WHILE app_running:
IF user_adds_transaction:
save_local(transaction)
IF online: sync_with_server()
IF sync_success: mark_local_synced()
update_ui_totals()
END


---

## Installation Instructions
- Step 1: Downloading the app:
       - Go to the app store on your device.
       - Search for Load It Up.
       - Tap: Install.
- Step 2: Setting Up Your Permissions
       - Open the app after it finishes installing.
       - Allow access to financial account data, behavorial and spending data, and third-party sharing and data usage.
       - When asked for Battery Optimization, select "Allow" (this ensures the app doesn't turn off when your screen is dark).
- Step 3: Logging In & Starting
       - Make your account (personal identification, secure authentication and financial account credetials).
       - Set up app and start session.
---

## Tech Notes
- Local storage (SQLite or JSON) with background sync  
- Minimal permissions required (storage, network)  
- Supports PDF/CSV export when online  

---

## Current project status
- Summary:
      - In developmental phase, everything completed is functional and requires only a few changes.
- Completed:
      - Backend setup: server is functional and is capable of processing data.
      - Database: Local storage (SQLite or JSON) is configured to store financial and behavioural data.
      - App UI: Created the Login and loading screens in the mobile app.
- In progress:
      - Live tracking of finances and purchases.
      - Testing: Running "dead zone" tests to see how the app behaves without Wi-Fi.
- Issues:
      - Access is limited.
      - Battery drain.
- Upcoming:
      - Finalize the "Monthly summary" screen and display.
      - Add automated SMS notifications when load arrives/is available.

--- 

## Contributors
Pie, Ma. Alicia Fatima E.  
Porio, Jahziel Christy R.  
Beltran, Justin Peter Noel B.
