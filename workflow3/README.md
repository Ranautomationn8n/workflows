# 🏥 Medical Appointment Automation (n8n Workflow)

This project is a fully automated appointment-booking system built in n8n. It streamlines how clinics handle patient requests for medical exams, ensuring accuracy, speed, and minimal manual work.

![screenshot](./workflow3/Screenshot2025-10-23151437.png)

📌 Overview

The workflow automates the entire process of collecting patient information, organizing appointments, and scheduling events based on exam type. No AI agents were used — everything is built with standard n8n nodes.

⚙️ How It Works
1. Patient Form Submission

Patients requesting:

Radiology

Echography

Echocardiogram

fill out an online form containing their details and preferred appointment date.

Once submitted, the data is automatically sent to a Google Sheet managed by the clinic administrator.

2. Automatic Calendar Scheduling

Depending on the exam type, the workflow proceeds as follows:

✔️ Radiology & Echography

A Google Calendar event is created immediately.

The appointment is added to the administrator’s calendar with the provided details.

✔️ Echocardiogram (Special Rule)

Echocardiograms can only be performed on Saturday or Sunday.

The workflow:

Checks the selected date.

If the date is Saturday or Sunday, it creates the event normally.

If the date is invalid (Monday–Friday), an automated email is sent to the patient asking them to resubmit the form and choose a weekend appointment.

📬 Automatic Email Handling

If the patient chooses the wrong day for an echocardiogram, the workflow:

Sends a polite email explaining the issue.

Asks the patient to refill the form.

Provides a link to reschedule correctly.

📊 Data Logging

All patient submissions — regardless of exam type — are stored neatly in a Google Sheet for easy administration, tracking, and reporting.
