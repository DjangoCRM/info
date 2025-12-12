---
title: Working With Deals in Django CRM
description: Learn how to effectively manage deals in Django CRM, including understanding the deal page layout,
  using interface actions, and utilizing deal data for sales analytics and reporting.
---

# **Working With Deals in Django CRM**

The Deal page in CRM is your central workspace for managing the full sales process —
from initial inquiry to final payment. This page collects key client information, communication history,
workflow steps, and financial data to help sales teams work efficiently and keep all deal-related information organized.

Below is a detailed overview of each section and function available on the Deal page.

---

## **Interface Actions and System Behavior**

### Gray-Button Actions

**(Do not save or modify deal data)**  
Some buttons on the Deal page are designed for creating related objects without altering the deal itself:

- **Office Memo** – Creates an internal memo linked to the current deal. Each memo includes a shortcut for users with access to quickly open the deal.
- **Message** – Opens a chat message form.

  - If the chat already contains messages, a *View chat* button appears.
  - If there are unread messages, the button turns **red**.

### Email Synchronization

CRM automatically syncs the assigned salesperson’s mailbox using deal tickets embedded in emails.  
At the bottom of the deal page, you’ll see the **four latest emails**.
Use the **two-envelopes icon** to view the full list of email correspondence.  
If an incoming email did not include a deal ticket, you can attach it manually using the **Import** button.

### Additional Tools

- **Deals** – Shows the number of deals associated with the same client. Clicking opens the full list.
- **Reminder (clock icon)** – Creates a reminder related to this deal. All reminders can be viewed in the **Common** section.
- **History** – Displays the full audit log: who changed what, when, and how.

---

## **Section 1: Main Information**

Here you can manage basic deal attributes:

- **Deal name** – Editable at any time. By default, inherited from the originating request.
- **Request information** – View key details from the request. Click **Request** to open it.
- **Important flag** – Highlight the deal in the Deal Manager and enable filtering by importance.
- **Closing the deal** – Select a closing reason from the drop-down list to close the deal.

*Related topic* - [Managing Requests](commercial-requests-management.md)

---

## **Section 2: Contact Information**

This section shows whom you're working with and provides quick communication tools:

- **Contact or Lead** – View the person involved in the deal and navigate to their profile.
- **Communication shortcuts:**

  - Send an **email**
  - Message via **WhatsApp**
  - Message via **Viber**
- **Company website** – Open the customer’s website.
- **Company profile** – Navigate to the customer’s company page.

*Related topics:*

- [Managing Leads](lead-management.md)
- [Managing Contacts](contact-management.md)
- [Managing Companies](company-management.md)

---

## **Section 3: Deal Progress and Workflow**

This section supports the operational management of the sales process:

### Stage Management

Select the current **deal stage** from the predefined list. These stages are used to build Sales Funnel report.

### **Financial Fields**

- **Total amount and currency** – The overall value of the deal.
- After adding payments, the CRM automatically calculates:

  - **Paid amount**
  - **Expected amount**

### Next Step Planning

- **Next step** – Briefly describe the upcoming action.
- **Step date** – Select the deadline.
- **Remind me** – Automatically creates a reminder.

### Workflow and History

- **Workflow** – Lists completed actions as the deal progresses.
- **Description** – Space for internal notes.
- **Stage dates** – Automatically populated list of completed stages with dates.

---

## **Section 4: Advanced Data and Linkages**

### Labels

Attach labels to categorize and filter deals more efficiently.

### Deal Connections

The deal displays its links to:

- Contact person and company (or lead)
- Partner representative (if applicable)
- Request

**Important:**
For accurate customer analytics, always specify the **end customer** in the contact and company fields — even if the sale is made through a partner. This can be adjusted later if the end customer becomes known.
Specifying a partner allows you to see all deals with this partner in the Deal manager using the partner filter.

### Additional Information

This area shows:

- Deal owner and co-owner (responsible sales managers)
- Last modified information (who last changed the deal and when.)
- Deal ticket

### Outputs (Products / Services)

Here you can describe what you're selling:

- Quantities and prices
- Contract and actual shipment dates
- Serial numbers (if applicable)
- Shipment status

### Payments

Add and track payment details:

- Payment amount and currency
- Actual or expected payment date
- Payment status (received / guaranteed / high probability / low probability)
- Contract and invoice numbers
- Order number
- Indicator for payments via representative office

### Files

Upload contracts, specifications, invoices, and other deal-related files.

---

## **Why Accurate Deal Data Matters**

Django CRM uses deal information to generate powerful marketing and analytical reports:

### Closure Reasons Report

Helps identify why deals fail and reveals patterns that impact sales performance.

### Sales Funnel Report

Based on the **Stage** field. Shows at which stage most deals are lost — for example, deals that never progressed beyond the price offer stage.

### Income Summary Report

Uses payment statuses to build revenue forecasts for the current and next two months.

### Sales Report

Shows which products or services were sold, when, by whom, and at what price.

If you need to update preset values for deal stages or closing reasons, contact your CRM administrator — these lists can be customized to match your business processes.
