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
- Option 1: Open index.html directly in a web browser for local testing.
- Option 2: Use a local development server (e.g., with Python):
   ```bash
   python -m http.server 8000
   ```
   Then navigate to http://localhost:8000 in your browser.
- Option 3: Deploy to a web server (e.g., Apache, Nginx) by copying index.html and styles.css to the server's root directory.

3. **Ensure File Paths:**
The styles.css file must be in the same directory as index.html for the <link rel="stylesheet" href="styles.css"> to work. If placed in a subdirectory (e.g., css/styles.css), update the href attribute in index.html accordingly.

## Usage

- Open the form in a browser to fill out patient details, medical history, appointment preferences, and insurance information.
- The form includes real-time validation (e.g., alphabetic names, valid phone numbers) and conditional fields (e.g., insurance details appear only if "Yes" is selected for insurance).
- Selecting "Emergency" in the urgency dropdown displays a warning to call 911 instead of submitting the form.
- Consent checkboxes for privacy and HIPAA are required before submission.
- Submit the form to send data to the specified endpoint (https://example.com/submit-appointment). Update the action attribute in index.html to point to your actual backend endpoint.

## Development

- HTML: The form is structured in index.html with semantic elements and ARIA attributes for accessibility.
- CSS: Styles are defined in styles.css with a warm, health-focused color palette and responsive design for mobile devices (media query for screens below 768px).
- JavaScript: Embedded in index.html to handle conditional field visibility and form submission validation (e.g., ensuring consent checkboxes are checked).

## Deployment

- Ensure index.html and styles.css are uploaded to the same directory on your web server.
- Update the form's action attribute to point to your backend API or server endpoint for processing form submissions.
- Test the form thoroughly to ensure all fields, validations, and conditional logic work as expected.

## Future Improvements

- Add backend integration for form submission processing and data storage.
- Implement advanced form validation (e.g., email format, file size limits).
- Enhance accessibility with additional ARIA roles and keyboard navigation.
- Separate JavaScript into an external file for better maintainability.
- Add unit tests for JavaScript functionality.