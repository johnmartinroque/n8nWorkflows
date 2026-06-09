# n8n Workflow Portfolio

A collection of workflow automations built with n8n to streamline HR, document management, and business processes.


---

# 1. File Upload to SharePoint

### Purpose

Automates the transfer of employee onboarding documents from Monday.com to SharePoint.


### Workflow Process

1. Triggered when onboarding documents are uploaded to a Monday.com item.
2. Retrieves employee details and attached files.
3. If only one file exists:

   * Uploads the document directly to SharePoint.
   * Renames it using the format:
     `Item Number - Employee Name`
4. If multiple files exist:

   * Combines all documents into a ZIP file.
   * Uploads the ZIP archive to SharePoint.
   * Uses the same naming convention:
     `Item Number - Employee Name.zip`

### Key Features

* Automatic file transfer
* Standardized naming convention
* Multi-file ZIP packaging
* SharePoint integration
* Reduced manual HR processing

### Workflow Diagram

<img width="1171" height="479" alt="File Upload - Monday com to Sharepoint Workflow" src="https://github.com/user-attachments/assets/f789ae8e-ba2e-4a53-9da7-3731e7f314fe" />


---

# 2. Service Agreement - Sent 

### Purpose

Tracks when a service agreement is successfully sent and updates related records automatically.


### Workflow Process

1. Detects when a service agreement is sent.
2. Updates the corresponding record.
3. Logs activity for reporting.
4. Notifies relevant stakeholders.

### Key Features

* Automated status updates
* Activity logging
* Stakeholder notifications
* Reduced manual tracking

### Workflow Diagram

![Service Agreement Sent](images/service-agreement-sent.png)

---

# 3. Service Agreement - Viewed Tracking

### Purpose

Monitors recipient engagement by detecting when service agreements are viewed.

### Business Problem

Sales and operations teams need visibility into document engagement without manual follow-up.

### Workflow Process

1. Receives document view events.
2. Identifies the recipient.
3. Updates workflow status.
4. Triggers follow-up actions if required.

### Key Features

* Real-time view tracking
* Automated status updates
* Follow-up automation
* Improved visibility

### Workflow Diagram

![Service Agreement Viewed](images/service-agreement-viewed.png)

---

## Workflow Summary

| Workflow                   | Purpose                       | Integrations                |
| -------------------------- | ----------------------------- | --------------------------- |
| File Upload to SharePoint  | Employee document management  | Monday.com, SharePoint      |
| Service Agreement - Sent   | Agreement delivery tracking   | E-signature platform, Email |
| Service Agreement - Viewed | Recipient engagement tracking | E-signature platform, Email |

## Contact

Feel free to connect if you'd like to discuss workflow automation, process optimization, or n8n development.
