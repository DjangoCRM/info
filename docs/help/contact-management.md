---
title: Managing Company Contacts
description: Learn how to manage company contacts in Django CRM, including contact creation, access permissions, 
  list overview, searching, filtering, bulk actions, and exporting data.
---

# **Managing Company Contacts in Django CRM**

Managing company contacts is one of the core features of [CRM](../index.md). The **Contacts** section in CRM allows users to store, organize, and work with information about employees and representatives of client companies. This guide explains how contacts appear in the CRM, how to manage them, how to use filters and bulk actions, and how to understand contact statuses.

> For related topics, see **[Company Management](company-management.md)**

---

## **What a Contact Represents**

A **Contact** is an individual person — an employee or representative of a client company. Contact records store key communication details and are used for sales processes, support, and email marketing campaigns.
Each contact is linked to a company, assigned to a sales manager, and included in newsletters or mass mailings.

---

## **How Contacts Are Added to CRM**

Django CRM supports several ways to add contacts to the system:

### 1. Automatic creation

Contacts can be created automatically when a user creates a **deal**, based on sales request data.

### 2. Manual creation

Users can manually add new contacts:

1. Click **Add Contact**.
2. Fill out the form with the required personal and company information.
3. Save the contact.

### 3. Import from Excel

If you need to upload contacts in bulk:

1. Click the **Import** button.
2. Select an Excel file prepared according to the CRM’s import format.
3. Upload it to add the contacts to the system.

### 4. Conversion from Lead

When a **Lead** is converted into a company and contact, CRM automatically creates a **Contact** record.

> Learn more: **[Lead Management](lead-management.md)**

---

## **User Access to Contacts**

Access to the contacts database depends on a user’s role and department:

- **Sales managers and operators**  —  access only contacts belonging to their own department.

- **Company managers and super operators**  — access all contacts across all departments.

This ensures that sensitive data is available only to authorized team members within the organization.

---

## **Working With the Contacts List**

The contacts list appears in a **sortable table**, allowing users to quickly organize and locate necessary information. Clicking on an active column header will sort contacts by that field.

### Table Columns

The table includes the following fields:

- Contact name
- Email
- Phone number
- Company name
- Country
- Status as a newsletter recipient
- Date added to CRM
- Assigned sales manager

Sorting and structured data improve speed and efficiency when working with large client databases.

---

## **Newsletter Subscription Status Indicators**

Next to each contact, a mailbox icon indicates their newsletter subscription status:

- **Red** — The contact has **not received any newsletters** yet.
- **Turquoise** — The contact **receives newsletters** and has **not unsubscribed**.
- **Gray** — The contact has **received newsletters** but has **unsubscribed**.

These visual markers help identify mailing preferences at a glance.

---

## **Searching and Filtering Contacts**

### Search bar

Use the search bar to find contacts by:

- Keywords (name, email, company, etc.)
- Contact ID

### Available filters

You can filter the contact list by:

- Department (if user role allows)
- Assigned sales manager
- Company industry
- Company type
- Country
- Newsletter subscription status
- VIP status
- Tags

These filters allow precise segmentation for sales analysis and marketing campaigns.

---

## **Bulk Actions for Contacts**

The **Action** dropdown menu allows users to perform mass operations on selected contacts:

- Create a **mass mailing**
- Set **VIP** status
- Remove **VIP** status
- **Export** selected contacts to Excel

Note: Users can export only the contacts assigned to them.

---

## **Mass Mailing Options**

There are two ways to create mass email campaigns from the Contacts page:

-  **1. Mass mailing for selected contacts**

Use the **Action → Make massmail** option.

- **2. Mass mailing for large groups**

Use the **Make massmail** button at the top to start a campaign for many contacts at once.

---

## **Exporting Contacts**

You can export contact data in two ways:

### Export selected contacts

Use the **Action → Export** option.
Users may export only the contacts they are responsible for.

### Export all contacts

To download the entire list (users can only export contacts assigned to them), use the **Export All** button.

---

> Recommended reading: [CRM application features](../features/crm-app-features.md)  
> For more on mailings, see [Email Campaigns and Newsletters](../features/massmail-app-features.md)