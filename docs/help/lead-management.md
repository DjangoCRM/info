---
title: Lead Management
description: Learn how to manage leads in Django CRM, including lead creation, access permissions, lead list overview, searching, filtering, bulk actions, and exporting data.
---

# **Lead Management**

The **Lead** object in Django [CRM](../index.md) represents a potential client.
A lead may be an individual or a partially completed company/contact profile
that has not yet been converted into Company and Contact Person.
Effective lead management ensures that sales teams can qualify prospects,
enrich their data, and convert relevant leads into companies and contacts.

This page explains how to view, manage, filter, sort, and convert leads inside Django CRM.

---

## **What Is a Lead?**

A lead contains basic information about a potential customer. The data may come from:

- Website requests
- Form submissions
- Manually added entries
- Automatically created leads when a sales manager creates a **Deal**

If missing information about a company and contact person is received during the processing of a sales request,
the Lead can be converted into a Company and Contact Person objects.

> For details on working with requests, see
**[Commercial Requests Management](../features/crm-app-features.md#commercial-requests-management)**.

---

## **Adding Leads to the CRM**

Leads can enter the CRM in several ways:

### 1. Automatic Lead Creation

When a deal is created from an incoming query and the CRM
detects insufficient customer data, a Lead is created automatically.

### 2. Manually Adding a Lead

Users can add leads manually:

- Click **Add Lead**.
- Fill in the form fields and save.

### 3. Importing Leads from Excel

You can upload multiple leads at once:

1. Click **Import**.
2. Select an Excel file prepared according to the CRM’s import format.
3. Confirm the upload.

For exporting options, see the **Exporting Leads** section [below](#exporting-leads).

---

## **Access Permissions**

Lead visibility depends on the user’s CRM role and department:

- **Sales Managers** and **Operators** — can view and manage leads assigned to *their own department*.
- **Company Managers** and **Super Operators** — have access to *all leads across all departments*.

---

## **Lead List Table**

Leads are displayed in a sortable table. Each column header is active, allowing you to sort leads by the selected field.

### Table Columns

- Lead Name / Full Name
- Email Address
- Company Name (*if any*)
- Assigned Sales Manager
- Country
- Newsletter Status
- Date Added

### Newsletter Status Icons

The lead’s position in your mailing activity is indicated by the color of the mailbox icon:

- **Red** — The lead has not yet received any newsletters.
- **Turquoise** — The lead receives newsletters and has not unsubscribed.
- **Gray** — The lead received newsletters but unsubscribed.

---

## **Searching Leads**

Use the search bar to find leads by:

- Name
- Email
- Company
- Any keyword
- Lead ID

---

## **Filtering Leads**

The CRM provides several filters to narrow down the lead list:

- Disqualification status
- Assigned sales manager
- Country
- Newsletter subscription status
- VIP status

Filters can be combined for more precise results.

---

## **Bulk Actions (*Action Menu*)**

Select one or more leads to perform bulk operations from the **Action** drop-down menu:

- Create Mass Mailing
- Set VIP Status
- Remove VIP Status
- Export to Excel

These actions help manage large lead lists efficiently.

---

## **Exporting Leads**

You can export lead data in Excel format:

### Export Selected Leads

Choose leads using the table checkboxes, then select **Export to Excel** from the Action menu.

### Export All Leads

Use the **Export All** button to download the complete lead database.

