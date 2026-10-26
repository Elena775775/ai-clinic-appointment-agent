# AI Clinic Appointment & Reporting Agent

## Project Overview

This project is an AI-powered clinic assistant built with **n8n**, **Telegram**, and **Google Sheets**. It automates appointment scheduling for patients and provides clinic management with reports on doctors' workload and appointment statistics.

The project was developed as a learning and portfolio project using fictional clinic data.

## Key Features

### 1. AI-Powered Appointment Booking
- Communicates with patients through Telegram.
- Retrieves doctors' information and specializations from Google Sheets.
- Checks existing appointments for the selected doctor and date.
- Guides patients through the booking process.
- Saves confirmed appointments to Google Sheets.
- Sends appointment notifications to the doctors' Telegram group.
- Confirms successful bookings to patients.

### 2. Automated Management Reporting
- Retrieves doctor schedules, salary data, and appointment records.
- Calculates scheduled hours, worked hours, workload utilization, and idle time.
- Estimates bonuses based on predefined workload thresholds.
- Calculates the estimated cost per worked hour.
- Sends structured reports to the clinic director through Telegram.

## Workflow Architecture

**Patient Booking Flow**

`Telegram → AI Agent → Google Sheets → Appointment Confirmation & Doctor Notification`

**Management Reporting Flow**

`Telegram → Reporting AI Agent → Google Sheets → Metrics Calculation → Telegram Report`

## Technology Stack

- **n8n** — workflow automation and orchestration
- **AI Agents and Language Models** — natural-language interaction and tool selection
- **Telegram Bot API** — patient communication and internal notifications
- **Google Sheets** — doctor directory and appointment database
- **JavaScript** — workload metrics calculations

## Testing

The workflows were tested using fictional project data, including appointment booking, Google Sheets record creation, Telegram notifications, and management queries about individual doctors.

## Business Logic

The reporting workflow uses predefined assumptions for monthly scheduled hours, workload utilization, idle time, and bonus thresholds. These are demonstration rules for this project and are not intended as universal payroll or healthcare standards.

## Demo Data

[Open Google Sheets — Clinic CRM (Doctors & Appointments)](https://docs.google.com/spreadsheets/d/1a5lMlQXvNnh3mrvA1fmELKRu8HKQnnbQiPDvGsU-7Qo/edit?usp=sharing)

The spreadsheet contains the demo data used by the appointment booking and reporting workflows.
## Project Files

- `README.md` — project overview and documentation
- `workflow.json` — sanitized n8n workflow export
- `screenshots/` — workflow screenshots

## Privacy & Limitations

This is an educational prototype, not a production-ready healthcare system. The public version should use fictional data and sanitized credentials and identifiers. Real patient data must not be included in the public repository.

The exported workflow requires appropriate credentials and configuration before it can run in another n8n environment.

## Author

Data Analytics & AI Automation Portfolio Project
