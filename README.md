# n8n-task-reminder-automation

Automated task reminder system built with **n8n** that reads tasks from Google Sheets, sends scheduled email reminders based on due dates, and updates task status automatically.

---

## Overview

This project demonstrates an automated workflow built using **n8n** to manage task reminders using **Google Sheets and Email notifications**.

The workflow checks tasks from a Google Sheet on a scheduled interval, calculates remaining days to the due date, sends reminder emails when required, and updates the sheet automatically.

This automation reduces manual tracking and helps ensure tasks are completed on time.

---

## Features

- Scheduled workflow execution
- Reads tasks from Google Sheets
- Calculates remaining days to deadline
- Sends automated reminder emails
- Prevents duplicate reminders
- Updates reminder status in the sheet
- Supports multiple reminder stages:
  - 3 days before due date
  - 1 day before due date
  - On the due date

## Workflow Logic

The automation performs the following steps:

1. A **Schedule Trigger** runs the workflow daily.
2. The workflow reads tasks from **Google Sheets**.
3. A **Code Node** calculates remaining days and determines whether a reminder should be sent.
4. If conditions match, the workflow sends an **email reminder**.
5. The sheet is updated with:
   - Reminder status
   - Reminder type
   - Last reminder date

---

## Reminder Conditions

The system sends reminders at:

- **3 days before the due date**
- **1 day before the due date**
- **On the due date**

Completed tasks are skipped to prevent unnecessary notifications.

---

## Technologies Used

- **n8n** – Workflow automation platform  
- **Google Sheets** – Task data storage  
- **Email Node** – Sending reminder emails  
- **JavaScript (Code Node)** – Reminder logic and date calculation  

---

## Use Cases

This automation can be used for:

- Task tracking
- Project deadline reminders
- Team follow-ups
- Personal productivity systems

---

## Future Improvements

Possible enhancements include:

- Slack or Microsoft Teams notifications
- AI-generated reminder messages
- Priority-based reminders
- Overdue task detection
- Dashboard reporting

---

## Author

Built as a workflow automation project using **n8n and Google Sheets** to explore practical automation for everyday task management.
