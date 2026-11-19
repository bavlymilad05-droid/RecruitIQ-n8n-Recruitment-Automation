# RecruitIQ – AI-Powered Recruitment Automation

RecruitIQ is an AI-powered recruitment automation system built with n8n. It automates job application intake, CV screening, candidate evaluation, and error monitoring.

## Live Website

https://bavlymilad05-droid.github.io/RecruitIQ-n8n-Recruitment-Automation/

## Workflows

### 1. Intake
- Trigger: n8n Form Trigger
- Validates candidate information and PDF CVs
- Detects duplicate applications
- Uploads CVs to Google Drive
- Records applications in Google Sheets

### 2. AI Scan
- Trigger: Hourly Schedule Trigger or Manual Trigger
- Extracts text from PDF CVs
- Uses Google Gemini for candidate screening
- Evaluates candidates against job requirements
- Generates scores and recommendations
- Sends automated email notifications

### 3. Error
- Trigger: Error Trigger and Schedule Triggers
- Monitors workflow failures
- Classifies errors by severity
- Sends critical error alerts
- Generates daily error reports
- Detects delayed applications

## Technologies

- n8n
- Google Gemini AI
- Google Sheets
- Google Drive
- Gmail
- JavaScript
- ngrok
- GitHub Pages

## Setup

1. Install and configure n8n.
2. Import the three JSON templates from the `workflows` directory.
3. Configure Google and AI credentials in n8n.
4. Replace placeholder IDs with your own Google Sheets and Drive IDs.
5. Configure the Error workflow for error handling.
6. Publish the workflows, starting with Error.
7. Configure the public Form URL and test the system.

## Notes

The published JSON files are sanitized workflow templates. Credentials and service identifiers must be configured before running imported workflows.

The live demo requires the locally hosted n8n instance and ngrok tunnel to be running.

## Project Purpose

This project demonstrates practical AI integration, workflow automation, document processing, recruitment decision support, and automated system monitoring.
