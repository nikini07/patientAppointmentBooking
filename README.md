# HealthLink Patient Appointment Booking

## Overview

HealthLink Patient Appointment Booking is a web-based form designed to streamline patient registration and appointment scheduling for HealthLink Clinic. The form addresses real-world issues such as long wait times and manual paperwork by providing a secure, accessible, and user-friendly online solution. It includes comprehensive patient details, medical history, symptom checker, insurance information, file uploads, conditional fields, real-time validation, and privacy consent features.

## Features

- Personal Details: Collects first name, last name, date of birth, gender, email, phone, and address with input validation.
- Medical History: Allows patients to input allergies, medications, past conditions, and select common conditions via checkboxes.
- Appointment Details: Includes department selection, preferred doctor, reason for visit, and urgency level with a conditional emergency warning.
- Insurance and Payment: Captures insurance details with conditional fields based on user input.
- Preferred Date & Time: Supports date, time, and appointment type (in-person or telemedicine) selection.
- Attachments and Consent: Enables file uploads for ID/insurance cards and medical records, with required consent checkboxes for privacy and HIPAA.
- Accessibility: Uses ARIA labels for screen reader support and a responsive design for mobile compatibility.
- Styling: Warm, accessible color scheme (forest green, muted brown, beige) with a clean, modern layout.
- Interactivity: JavaScript for conditional field visibility (e.g., insurance details, emergency warning) and form validation.

## File Structure

## File Structure

```plaintext
patientAppointmentBooking/
├── index.html         # Main HTML file containing the form structure and JavaScript
├── styles.css         # External CSS file for styling the form
├── README.md          # Project documentation
└── LICENSE            # MIT License file
```

## Setup Instructions

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/<your-username>/patientAppointmentBooking.git
   cd patientAppointmentBooking

2. **Serve the Application:**
Option 1: Open index.html directly in a web browser for local testing.
Option 2: Use a local development server (e.g., with Python):
   ```bash
   python -m http.server 8000