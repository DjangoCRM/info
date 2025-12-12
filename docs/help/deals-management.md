---
title: Managing Deals
description: Learn how to manage deals in Django CRM, including deal creation, access permissions, deal list overview, searching, filtering, and exporting data.
---

# **Managing Deals**

The **deal** is the main [CRM](../index.md) object used by sales managers to
track commercial work with potential and current customers.
It stores the full history of communication, negotiation, and decision-making —
from the initial [request](request-processing.md) to the successful closing (or rejection) of the deal.

This page explains how to work with the deal list and use available tools for
organizing and analyzing sales activities.

---

## **Deal Creation and Access Permissions**

For marketing analysis purposes, a deal can only be created **based on a request**
received from a website form, email, or created manually within the CRM.

➡ Note: The products or services specified in the request may differ from what the deal
is ultimately closed for.

Access to deals is regulated by user roles and departments:

| Role               | Access Level                     |
| ------------------ |----------------------------------|
| Sales Manager      | *Deals within their department*  |
| Company Executives | *All deals from all departments* |
| Other Users        | *Do not have access to deals*    |

For teams in small businesses, CRM allows users to combine roles:
operator, sales manager, and even company manager.  
If you need role changes or custom permissions, please contact your **CRM Administrator**.

---

## **Deal List Overview**

The deal list is displayed as a sortable table with active column headers. Columns include:

- **Deal Name** — inherited from the request but can be edited.
- **Next Step** — what action needs to be taken next.
- **Next Step Date** — deadline for the planned action.
- **Stage** — current progress status.
- **Name of counterparty (lead or company)** — clickable link to the counterparty page.
- **Counter** — the number of deals with this counterparty in the CRM database.
- **Sales Manager** — assigned responsible user.
- **Active** — whether the deal is currently being worked on.
- **Deal Relevance Flag**.
- **Creation Date**
- **Deal ID**

---

## **Deal Status Icons**

Icons provide quick information about deal conditions:

- No reply has been sent yet to the customer request.
- Payment has been received.
- No products/services are listed in the deal.
- Payment received but shipping/service date not specified.
- Shipping/service deadline expired.
- Files attached to the deal.

Hover your cursor over any icon to see a tooltip with details.

---

## **Searching and Filtering Deals**

### Search

Use the **search bar** to find deals by:

- Keywords
- Deal ID

### Filters

A **filter panel** helps narrow down the list dynamically. Available filters include:

- Department (if role allows selection)
- Importance rating
- Sales manager (owner)
- Product or service
- Partner (sales representative)
- Modified by company management
- Relevance indicator
- Creation date
- Deal stage
- Reason for closing
- Customer industry
- Labels / tags

Filters can be combined to refine results further.  
By default, only active deals are displayed in the list.

---

## **Exporting Deal Data**

Using the **“Action”** drop-down menu, you can export selected deals to an **Excel file**.
This is especially useful for data sharing or reconciliation with trading partners.

---

## Related Topics

- [Working with Deals](working-with-deals.md)
- [Managing Commercial Requests](commercial-requests-management.md)  
- [CRM Software Overview](../features/overview.md)