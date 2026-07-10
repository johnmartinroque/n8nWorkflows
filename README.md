# n8n Workflow Portfolio

A collection of workflow automations built using n8n to streamline internal business processes, document management and notifications

---



## 1. Data Analyst & Report Email AI Agent

<img width="1163" height="490" alt="image" src="https://github.com/user-attachments/assets/f1a5ca84-55f0-46fe-82e5-d6c5174189b4" />



### Overview

An AI-powered data analysis assistant that enables users to interact with an e-commerce order dataset through natural language. The workflow retrieves live data from Google Sheets, performs calculations, generates professional PDF reports, and delivers analysis via email.

### Key Features

* Provides conversational data analysis using natural language queries.
* Retrieves live order data directly from Google Sheets.
* Performs calculations including:
  * Revenue
  * Sales totals
  * Average order value
  * Product performance
  * Regional sales analysis
* Automatically generates professionally formatted HTML reports.
* Converts reports into PDF documents.
* Sends reports via email with a secure PDF download link.
* Maintains conversation context using AI memory for follow-up questions.
* Ensures all analyses are based on the latest spreadsheet data.

### Integrations Used

* n8n AI Agent
* Google Gemini
* Google Sheets
* Calculator Tool
* PDF.co
* SMTP Email
* JavaScript
* Memory Buffer

## 2. Employee Document Upload to SharePoint

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

## 3. Service Agreement Status Tracking — Sent

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

## 4. Service Agreement Status Tracking — Viewed

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

## 5. Service Agreement Status Tracking — Completed

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

## 6. Pricing File Upload Notification

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




## 7. Data Analyst & Report Email AI Agent

<img width="1163" height="490" alt="image" src="https://github.com/user-attachments/assets/f1a5ca84-55f0-46fe-82e5-d6c5174189b4" />



### Overview

An AI-powered data analysis assistant that enables users to interact with an e-commerce order dataset through natural language. The workflow retrieves live data from Google Sheets, performs calculations, generates professional PDF reports, and delivers analysis via email.

### Key Features

* Provides conversational data analysis using natural language queries.
* Retrieves live order data directly from Google Sheets.
* Performs calculations including:
  * Revenue
  * Sales totals
  * Average order value
  * Product performance
  * Regional sales analysis
* Automatically generates professionally formatted HTML reports.
* Converts reports into PDF documents.
* Sends reports via email with a secure PDF download link.
* Maintains conversation context using AI memory for follow-up questions.
* Ensures all analyses are based on the latest spreadsheet data.

### Integrations Used

* n8n AI Agent
* Google Gemini
* Google Sheets
* Calculator Tool
* PDF.co
* SMTP Email
* JavaScript
* Memory Buffer

