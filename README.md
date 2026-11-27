# AI Lead Qualification System

An AI-powered lead qualification and categorization system built using **n8n, Google Gemini, Google Sheets, and Gmail**.

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

The main workflow follows these stages:

1. Lead Data Retrieval
2. Data Validation
3. Lead Data Preparation
4. AI-Powered Analysis
5. AI Output Validation
6. Lead Categorization
7. CRM Updates and Email Notifications

A separate Error Handling Workflow is configured in the main workflow's settings to capture execution failures and send automated Gmail notifications.

## Error Handling Workflow

A separate n8n workflow that captures execution failures and sends automated email notifications with error details.

[Download Error Handling Workflow (JSON)](AI-Lead-Qualification-Error-Workflow.json)

## Sample Data Files

- [Sample CRM Input Data](Sample-CRM-Input-Data.csv) — Fictional CRM leads used to test the workflow.
- [Sample CRM Execution Output](Sample-CRM-Execution-Output.csv) — CRM records after workflow execution.

## Email Notifications

### Automated Lead Notifications

- **Hot Lead Notification:** Automated email sent for high-priority leads.
- **Warm Lead Notification:** Automated email sent for potential leads.

### Error Notification

- **Error Notification Email:** Example of an error alert successfully received by email through the separate error-handling workflow.

## Data Processing Notes

- **Invalid Leads:** Lead Score and AI qualification fields remain blank for invalid records because they are excluded from the AI qualification process.
- **Valid Leads:** Follow-up Status is intentionally not updated by the current workflow. Automated follow-up status management is outside the current implementation scope.

These behaviors are intentional and reflect the current workflow design.

## Project Status

Developed and tested as a practical AI automation project using fictional lead data.

## Limitations

- The workflow was developed and tested in a local n8n environment.
- AI-generated scores and categories require human review before business decisions.
- Public live deployment is not currently available.

## Setup & Configuration

The workflow JSON files are sanitized portfolio templates and are not ready to run immediately after import.

To use the automation:

1. Install or access an n8n instance.
2. Import the main workflow JSON file.
3. Configure your own AI model credentials for Google Gemini.
4. Connect your Google Sheets account and configure your own CRM spreadsheet.
5. Connect your Gmail account and configure the required email recipient details.
6. Configure any required API credentials, webhook settings, and integration parameters.
7. Import and configure the separate error workflow.
8. Submit sample lead data and test the workflow.

**Note:** The exported workflow files do not contain working credentials or private account configurations. You must configure your own integrations before execution.

### Sample Data & Privacy

- All lead information provided in this repository is fictional and created for demonstration and testing purposes.
- No real customer or business information is intentionally included.
- Workflow JSON files are sanitized to remove private credentials and account-specific configurations.
- Use fictional or properly authorized test data when reproducing this project.

## Author

**AI Automation & Integration | Management Sciences Undergraduate Student at GIKI**

## Project Screenshots

### 1. Workflow Overview

![Workflow Overview](Workflow%20Overview.png)

### 2. Successful Execution

![Successful Execution](Successfull%20Execution.png)

### 3. CRM Input – Test Data

![CRM Input – Test Data](CRM%20Input%20-%20Test%20Data.png)

### 4. CRM Validated Leads Data

![CRM Validated Leads Data](CRM%20Validated%20Leads%20Data.png)

### 5. AI Lead Analysis (LLM Node)

![LLM Lead Analysis](AI-Lead-Analysis.png)

### 6. Post-AI Data Processing (Code Node)

![Post-AI Data Processing](Validate%20AI%20Results.png)

### 7. Lead Category Routing (Switch Node)

![Lead Category Routing Switch](Categorize%20Leads.png)

### 8. CRM Hot, Warm & Unqualified Leads

![CRM Hot, Warm & Unqualified Leads](CRM%20Hot,%20Warm%20&%20Unqualified%20Leads.png)

### 9. Hot Lead Notification

![Hot Lead Notification](Hot-Lead-Notification.png)

### 10. Warm Lead Notification

![Warm Lead Notification](Warm-Lead-Notification.png)

### 11. Error Handling Workflow

![Error Handling Workflow](Error-Handling-Workflow.png)

### 12. Error Notification Email

![Error Notification Email](Error-Notification-Email.png)

## Project Videos

The following videos demonstrate the project presentation, workflow execution, and practical functionality.

1. **Project Presentation & Workflow Execution:** [Watch Video 1](https://youtu.be/TrbrbRSboZI)

   *Note: Execution / Testing of workflow starts at 5:26.*

2. **Practical Workflow Demonstration:** [Watch Video 2](https://youtu.be/4glMDupIduA)

## Project Documentation & Presentation

Additional project materials are available below for a detailed understanding of the system's design, implementation, and workflow.

### Project Presentation

- [PowerPoint Presentation (PPTX)](AI-Lead-Qualification-System-Presentation.pptx)

### Project Documentation

[View Project Documentation (PDF)](AI-Lead-Qualification-System-Documentation.pdf)
