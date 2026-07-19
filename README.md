# n8n Workflow Portfolio

A collection of workflow automations built using n8n to streamline internal business processes, document management and notifications

---



## 1. Automated Monthly Business Reporting System

<img width="1217" height="427" alt="image" src="https://github.com/user-attachments/assets/fc54a91b-9d57-46d3-8c25-af9050dfa43a" />


### Overview

An AI-powered workflow that automatically generates monthly Sales & Inventory reports using live Google Sheets data. Scheduled to run on the first day of every month, the workflow analyzes business performance, creates a professionally formatted PDF report, stores it in Google Drive, and emails it to stakeholders.

### Key Features

* Automatically runs on a monthly schedule using a Cron trigger.
* Determines the current month and retrieves data from the corresponding Google Sheets worksheet.
* Uses Google Gemini AI to generate business insights and executive summaries.
* Performs calculations including:
  * Total Revenue
  * Total COGS
  * Gross Profit
  * Average Gross Margin
  * Units Sold
  * Low Stock Products
* Generates a professionally formatted HTML Sales & Inventory report.
* Converts the HTML report into a PDF using PDF.co.
* Uploads the generated PDF to Google Drive for centralized storage.
* Automatically emails the completed report as an attachment to stakeholders.
* Eliminates manual report preparation and ensures timely monthly reporting.

### Workflow Process

1. Executes automatically on the first day of each month.
2. Determines the current month.
3. Retrieves live sales and inventory data from the corresponding Google Sheets tab.
4. Uses Google Gemini AI to analyze business performance.
5. Calculates key business metrics using the Calculator Tool.
6. Generates a one-page HTML Sales & Inventory report.
7. Converts the report into a PDF.
8. Uploads the PDF to Google Drive.
9. Sends the completed report via email with the PDF attached.

### Integrations Used

* n8n AI Agent
* Google Gemini
* Google Sheets
* Google Drive
* PDF.co
* SMTP Email
* Schedule Trigger (Cron)
* Calculator Tool
* JavaScript


## 2. InsightForge – AI Business Intelligence Assistant

<img width="1184" height="456" alt="image" src="https://github.com/user-attachments/assets/02ff6c5e-d1e4-4302-a5f1-831e7e49015a" />


### Overview

InsightForge is an AI-powered business intelligence workflow built with n8n that enables users to analyze product data through natural language conversations. The workflow retrieves live information from Google Sheets, performs data analysis using Google Gemini, maintains conversational context, and returns structured responses with optional chart data for frontend visualization.

### Key Features

* Accepts natural language business questions through a webhook API.
* Validates incoming requests before processing.
* Uses Google Gemini AI to interpret analytical queries.
* Retrieves live product data directly from Google Sheets.
* Performs calculations including:
  * Product comparisons
  * Sales analysis
  * Inventory analysis
  * Category summaries
  * Average values
  * Counts and filtering
* Automatically determines when charts are appropriate.
* Returns structured JSON responses containing:
  * Business-friendly insights
  * Chart configuration for frontend rendering
* Supports multiple chart types:
  * Bar Charts
  * Line Charts
  * Pie Charts
* Maintains conversation history using AI memory for contextual follow-up questions.
* Includes response formatting and validation to ensure consistent API output.
* Provides error handling for invalid or incomplete requests.

### Workflow Process

1. Receives a user query through a webhook.
2. Validates that the request contains a message.
3. Sends the query to the AI Agent.
4. Retrieves relevant product data from Google Sheets.
5. Performs the requested calculations and analysis.
6. Generates structured JSON containing:
   * Natural language response
   * Optional chart data
7. Formats and validates the AI output.
8. Returns the response to the frontend through the webhook.

### Integrations Used

* n8n AI Agent
* Google Gemini
* Google Sheets
* Webhooks
* JavaScript
* Memory Buffer
* HTTP API


## 3. Employee Document Upload to SharePoint

<img width="1171" height="479" alt="File Upload - Monday.com to SharePoint Workflow" src="https://github.com/user-attachments/assets/f789ae8e-ba2e-4a53-9da7-3731e7f314fe" />

### Overview

Automates the transfer of employee onboarding documents from Monday.com to SharePoint.

### Key Features

* Supports both single and multiple file uploads.
* Processes onboarding documents such as:

  * NBI Clearance
  * Birth Certificate
  * Certificate of Employment
  * Medical Certificate
  * Other required onboarding files
* Automatically renames files using a standardized naming convention:

  * **Document Type + Employee Name + Item ID**
* Compresses multiple uploaded files into a single ZIP archive before storage.
* Uploads processed files directly to SharePoint for centralized document management.

### Integrations Used

* Webhooks
* HTTP
* JavaScript
* Monday.com
* SharePoint

---

## 4. Service Agreement Status Tracking — Sent

<img width="958" height="772" alt="Service Agreement - Sent Workflow Full View" src="https://github.com/user-attachments/assets/64b29f1d-8815-4658-86f5-ff11f761838c" />

### Overview

Tracks PandaDoc service agreements when documents are sent to clients.

### Key Features

* Monitors PandaDoc document status changes.
* Updates service agreement status to **Sent**.
* Records key information including:

  * Document Name
  * Client Name
  * Date Sent
* Synchronizes data to:

  * Microsoft Excel Client Tracker
  * Monday.com Client Tracker Board

### Integrations Used

* Webhooks
* HTTP
* PandaDoc
* JavaScript
* Monday.com
* Excel


---

## 5. Service Agreement Status Tracking — Viewed

<img width="845" height="693" alt="Service Agreement - Viewed" src="https://github.com/user-attachments/assets/4fab9eac-4d1d-47a2-b47b-73ab8bee7549" />

### Overview

Tracks when clients open and view service agreements.

### Key Features

* Detects PandaDoc document view events.
* Updates service agreement status to **Viewed**.
* Records:

  * Document Name
  * Client Name
  * Date Viewed
* Updates tracking records in:

  * Microsoft Excel Client Tracker
  * Monday.com Client Tracker Board

### Integrations Used

* Webhooks
* PandaDoc
* JavaScript
* Monday.com
* Excel

---

## 6. Service Agreement Status Tracking — Completed

<img width="1644" height="936" alt="Service Agreement - Completed" src="https://github.com/user-attachments/assets/21fab2be-d80f-411b-9111-f1b4c5b5a4f0" />

### Overview

Automates the final stage of the service agreement lifecycle after client completion.

### Key Features

* Detects completed PandaDoc agreements.
* Updates agreement status to **Completed**.
* Records:

  * Document Name
  * Client Name
  * Completion Date
* Updates data across:

  * Microsoft Excel Client Tracker
  * Monday.com Client Tracker Board
* Automatically assigns:

  * Account Manager
  * Point of Contact (POC)
* Ensures seamless handoff from sales to account management.

### Integrations Used

* Webhooks
* PandaDoc
* JavaScript
* Monday.com
* Excel

---

## 7. Pricing File Upload Notification

<img width="1588" height="936" alt="Pricing Upload Notification" src="https://github.com/user-attachments/assets/ac854c35-b509-4f8a-8dd7-bcf4383c2730" />

### Overview

Automates internal pricing notifications between recruitment and finance/sales teams.

### Key Features

* Detects newly uploaded pricing files.
* Sends pricing documents through the recruiter's Outlook account.
* Automatically notifies relevant finance and sales stakeholders.
* Eliminates manual email preparation and reduces communication delays.

### Technologies

* Webhooks
* Monday.com
* Microsoft Outlook
* HTTP
* JavaScript

## 8. AI-Powered Monthly Sales & Inventory Reporting System (With Format)

<img width="1600" height="900" alt="AI Monthly Sales & Inventory Reporting Workflow" src="YOUR_WORKFLOW_IMAGE_URL_HERE" />

### Overview

An AI-powered reporting workflow that automatically generates professional monthly Sales & Inventory reports from live Google Sheets data. Running on a scheduled trigger, the workflow analyzes sales performance using Google Gemini, calculates key business metrics, renders a polished HTML report, converts it into a PDF, stores it in Google Drive, and emails the completed report to stakeholders.

Unlike traditional reporting workflows, this version dynamically generates executive insights, profitability analysis, revenue visualizations, and business recommendations without requiring manual intervention.

### Key Features

* Automatically runs on the first day of every month using a Schedule Trigger.
* Determines the current reporting month automatically.
* Retrieves live sales and inventory data from Google Sheets.
* Uses Google Gemini AI to generate business analysis and executive summaries.
* Calculates business KPIs including:
  * Total Revenue
  * Total COGS
  * Gross Profit
  * Average Gross Margin
  * Total Units Sold
* Compares current and previous month performance when historical data is available.
* Identifies:
  * Top 3 Highest Margin Products
  * Top 3 Lowest Margin Products
* Generates revenue-by-category visualizations directly inside the report.
* Produces AI-generated business recommendations based on sales performance.
* Dynamically renders a professionally formatted HTML report using a custom template.
* Converts the HTML report into a high-quality PDF using PDF.co.
* Automatically uploads the finished report to Google Drive.
* Emails the PDF report to stakeholders as an attachment.

### Workflow Process

1. Executes automatically on a monthly schedule.
2. Determines the current month and report filename.
3. Retrieves live sales data from the corresponding Google Sheets worksheet.
4. Optionally retrieves previous month's data for performance comparison.
5. Uses Google Gemini AI to analyze sales performance and generate structured report data.
6. Calculates business KPIs and profitability metrics.
7. Renders a fully formatted HTML Sales & Inventory report.
8. Converts the HTML report into a PDF.
9. Downloads the generated PDF.
10. Uploads the report to Google Drive.
11. Sends the completed report via email with the PDF attached.

### Integrations Used

* n8n AI Agent
* Google Gemini
* Google Sheets
* PDF.co
* Google Drive
* SMTP Email
* Schedule Trigger
* JavaScript
* Calculator Tool

