---
title: Managing Companies
description: Learn how to manage companies in Django CRM, including company creation, access permissions, list overview,
  searching, filtering, bulk actions, and exporting data.
---

# **Managing Companies in Django CRM**

The **Company** object in the [CRM](../index.md) stores information about existing or potential client companies.
Accurate company data is essential for sales operations, segmentation, and marketing outreach.
This guide explains how to create companies, import company data, assign managers,
and filter your company list for efficient sales and marketing work.

---

## **What Is the Company Object in Django CRM?**

A Company record represents a client or potential client. It includes key business details such as name,
address, contact details,  type, registration number, assigned sales manager, newsletter status, and industry.
Maintaining accurate company profiles helps sales teams segment markets and manage the sales pipeline.

---

## **How Companies Are Added to the CRM**

Django CRM supports multiple ways to create or import companies:

### 1. Automatically when creating a deal

If the request contains information about a company and this company is not found in the CRM,
then when creating a [deal](deals-management.md), the Company record will also be automatically created.

### 2. Manual creation

You can add a company manually by clicking **Add Company** and completing the form.
Before creating a new company, check whether a **Lead** with the same company name already exists.

> See also: [Managing Leads in CRM](lead-management.md).

### 3. Import from Excel

To add multiple companies at once:

1. Click **Import**.
2. Select an Excel file prepared according to the CRM’s import format.
3. Upload it to create or update company entries.

### 4. Converting a Lead

When converting a Lead to a client, the CRM can automatically create a corresponding Company record.

---

## **Company Access Permissions**

Access to company records depends on user roles and departments:

- **Sales managers** and **operators** see only companies belonging to their own department.
- **Company managers** and **super operators** have access to companies across all departments.

If you do not see the company you expect, contact your CRM administrator to review your permissions.

---

## **Company List View and Table Fields**

All companies are displayed as a sortable table. Most column headers allow ascending/descending sorting.

### **Table Columns**

- **Company name**
- **Company type** *(distributor, dealer, reseller, customer end  competitor)*
- **Date added**
- **Assigned sales manager**
- **Country**
- **Newsletter recipient status**
- **Company ID**
- **Registration number**

These sets of types and industries can be adjusted to match your business specifics.
Contact your CRM administrator if customization is needed.

---

## **Newsletter Status Indicators**

The newsletter subscription status is shown as a colored mailbox icon:

- **Red** — The company has not yet received any newsletters.
- **Turquoise** — The company received newsletters and has not unsubscribed.
- **Gray** — The company unsubscribed from newsletters.

---

## **Searching for Companies**

Use the search bar to find companies by:

- Company name
- Keywords
- Company ID

Search results update instantly based on your input.

---

## **Filters for Company Database Management**

Use the filter panel to narrow down the list by:

- Department (based on your role)
- Presence of linked contact persons
- Assigned sales manager
- Last updated date
- Industry
- Company type
- Country
- Newsletter subscription status
- VIP status
- Tags

These filters help you segment companies for marketing, sales follow-up, or reporting.

---

## **Bulk Actions**

Select one or more companies and use the **Action** drop-down menu to perform group actions:

- **Create mass mailing** (email campaigns)
- **Set or remove VIP status**
- **Export selected companies to Excel**
- **Reassign companies to another sales manager** (role permitting)

Administrators can also transfer selected companies to another manager from this menu.

To transfer a single company along with its Contacts, change the **Owner** field on that company’s page.

---

## **Creating Mass Mailings**

There are two ways to launch a mass mailing:

- From the **Action** menu (for selected companies)
- Via the **Make massmail** button (for a large group)

---

## **Exporting Companies**

You can export company data using:

- **Export** (for selected rows)
- **Export All** — exports the entire company database to Excel

Users can only export companies assigned to them.

---

## Related Topics

- [Managing Commercial Requests in CRM](commercial-requests-management.md)  
- [CRM Email Marketing](../features/massmail-app-features.md)