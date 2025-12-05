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

## Tech Notes
- Local storage (SQLite or JSON) with background sync  
- Minimal permissions required (storage, network)  
- Supports PDF/CSV export when online  

---

## Contributors
Pie, Ma. Alicia Fatima E.  
Porio, Jahziel Christy R.  
Beltran, Justin Peter Noel B.
