# AI Lead Qualification System

An AI-powered lead qualification and categorization system built using n8n, Google Gemini, Google Sheets, and Gmail.

## Project Overview

The AI Lead Qualification System automates the process of reviewing, validating, analyzing, and categorizing business leads. It uses AI-powered analysis to help organize lead information and streamline follow-up processes.

## Business Problem

Manually reviewing and qualifying leads can consume time, create inconsistent assessments, and delay follow-ups. Businesses need a structured process to validate incoming lead data, prioritize potential customers, and manage lead records efficiently.

## Proposed Solution

This project uses n8n to automate lead processing. It retrieves lead records from Google Sheets, validates the data, analyzes valid leads using Google Gemini, and routes them according to their qualification categories.

## Technologies Used

- **n8n:** Workflow automation and orchestration
- **Google Gemini:** AI-powered lead analysis
- **Google Sheets:** CRM data storage and management
- **Gmail:** Automated email notifications
- **JavaScript:** Data validation and processing
- **JSON:** Structured data exchange
- **APIs and Webhooks:** Workflow integration and triggering

## Key Features

- Automated CRM lead retrieval
- Lead data validation
- AI-powered lead analysis and scoring
- Automated lead categorization
- Category-based workflow routing
- Google Sheets record updates
- Automated email notifications
- Error handling and workflow monitoring

## Workflow Architecture

The workflow follows these main stages:

1. Lead Data Retrieval
2. Data Validation
3. Lead Data Preparation
4. AI-Powered Analysis
5. AI Output Validation
6. Lead Categorization
7. CRM Updates and Email Notifications
8. Error Handling

## Project Status

Developed and tested as a practical AI automation project using fictional lead data.

## Limitations

- The workflow was developed and tested in a local n8n environment.
- AI-generated scores and categories require human review before business decisions.
- Public live deployment is not currently available.

## Author

**AI Automation & Integration | Management Sciences Student**

## Project Screenshots

### 1. Workflow Overview
![Workflow Overview](Worflow%20Overview.png)

### 2. Successful Execution
![Successful Execution](successful-execution.png)

### 3. CRM – Hot, Warm and Cold Leads
![Hot/Warm Leads](crm-hot-warm-leads.png)

### 4. CRM – Validated Leads Data
![Validated CRM Data](crm-validated-lead-data.png)

### 5. Invalid Leads
![Invalid Leads](invalid-leads.png)

