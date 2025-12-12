---
title: Managing Commercial Requests
description: Learn how to manage commercial requests in Django CRM, including user roles, access rights, request creation, and best practices.
---

# **Managing Commercial Requests**

Commercial requests in [Django CRM](../index.md) help sales teams track potential customers who are looking
for specific products or services. A request is often the first step toward creating
a deal and initiating the sales process.

This page explains how CRM users manage commercial requests, what access rights apply,
and how to work effectively with the request list.

> Related topics:  
> [Managing Deals in Django CRM](deals-management.md)  
> [Explore the CRM Application](../features/crm-app-features.md)

---

## **What are Commercial Requests?**

A request includes [essential details](request-processing.md) about a customer’s inquiry — what they want to purchase,
who they represent, and their contact information. These records can appear in the CRM in
several ways:

- **Automatically** from a website form
- **Automatically** from selected incoming emails (if configured)
- **Manually** added by a CRM user
- **Copied** from an existing request (to save time for recurring inquiries)

Keeping requests complete and accurate is important — correct contact data allows
the CRM to match companies, leads, and contacts already in the database.

---

## **User Roles Working With Requests**

There are **three roles** directly involved in request handling:

| Role              | Responsibilities                                         | Level of Access                 |
| ----------------- |----------------------------------------------------------|---------------------------------|
| **Operator**      | Processes requests, creates deals, assigns sales manager | Only within assigned department |
| **Super Operator** | Manages requests for all departments                    | All company requests            |
| **Sales manager** | Creates requests, creates deals                          | Only within assigned department |

If CRM is used for small businesses, the same person may act as both operator **and** sales manager.

Sales managers primarily work with **deals**, not requests. Operators convert qualified
requests into deals and assign them for further work. In cases where requests are
received directly by sales managers, they create the requests themselves. 

To change roles or request additional access, please contact your **CRM administrator**.

---

## **When Should a Deal Be Created?**

A deal represents the **active sales workflow** — not the closed contract. For most valid requests, a deal **must** be created.

A deal **is not created** only when the request is marked as:

* **Duplicate**
* **Case/Incident** (support request without commercial potential)
* **Irrelevant** (the field is hidden by default)

---

## **How to Add Requests**

Users with appropriate permissions can add requests:

| Method                        | How it works                                                                         |
| ----------------------------- | ------------------------------------------------------------------------------------ |
| **Add Request** button        | Opens a blank form — fill in all required details                                    |
| **Import Request from Email** | Creates a request from inbound email (email account must first be configured in CRM) |
| **Copy** button               | Creates a duplicate draft with editable data                                         |

Requests from website contact forms appear automatically in the system.

---

## **Managing the Request List**

All requests are displayed in a sortable table. Column headings include:

- **Request Name**
- **Loyalty Label**
  • *Primary*: Marketing-generated
  • *Subsequent*: Direct client contact by a known lead or company
- **Counterparty Name** (lead or company)
- **Country**
- **Contact Person**
- **Request Date**
- **Assigned Operator or Sales Manager**
- **Request Status** — *pending* or *processed*

### **Search and Filtering**

You can quickly find the needed requests using:

✅ **Search bar** — search by ID *(id123)* or keywords  
✅ **Filter panel** — filter by:

- Department (if allowed by role)
- Request status
- Assigned operator or sales manager
- Date received
- Product or service
- Loyalty
- Country

---

## **Access Rules Summary**

| User Type       | What They Can Access                          |
| --------------- | --------------------------------------------- |
| Operator        | Requests in own department                    |
| Sales Manager   | Requests in own department (assigned to them) |
| Super Operator  | Requests in all departments                   |
| Company Manager | Full visibility across the CRM                |

---

## **Best Practices**

* Review every new request promptly
* Verify client contact details
* Mark duplicates to avoid confusion in the sales pipeline
* Convert qualified requests into deals right away

> Recommended reading:
>
> * [Explore the CRM Application in Django CRM suite](../features/crm-app-features.md)
