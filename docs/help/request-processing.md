---
title: Request Processing
description: Learn how to effectively process commercial requests in Django CRM, including verifying request details,
  enriching missing information, linking to existing CRM entities, and creating deals or cases.
---

# **Request Processing in Django CRM**

Request processing ensures that every inbound client inquiry is converted into accurate, complete, 
and actionable CRM data. This page guides users through verifying request details, enriching missing information,
linking the request to existing CRM entities, and ultimately creating a deal or closing the request as a case.
Effective request processing strengthens data quality, reduces duplicates, and improves follow-up speed.

---

## **Purpose of request processing**

Request processing focuses on **verifying** and **enriching** client contact information before passing the inquiry to the sales pipeline.
Accurate request handling ensures the verification and completeness of customer data.
This serves two critical functions:

1. Ensuring the sales team can reach the client.
2. Matching the inquiry to existing CRM records to avoid duplicate [leads](lead-management.md),
  [contacts](contact-management.md), or [companies](company-management.md).

Most client [requests](commercial-requests-management.md) are generated automatically when a visitor submits a website form or sends an email.
Before the request becomes a deal, all information must be checked for accuracy and completeness.

Once **validated**, a deal must be created. For users with the operator role,
the request owner must be reassigned to a sales manager before creating the deal.
Note that deals cannot be created from requests marked as duplicates or as cases/incidents.

---

## **Request counter and assignment workflow**

The left-panel includes a request **counter** that helps CRM users track incoming workload.

- The green value shows the number of new pending requests that need processing.
- The red value indicates requests older than 24 hours that are still unassigned to a sales manager.

A request disappears from the counter once a sales manager is assigned as the owner.

---

## **Case and incident handling**

If a request does not require payment or sales follow-up, it must be marked as a **case/incident**.
This replaces the Create Deal button with a Close button.
Cases appear green in the request list and turn gray after closing. These items are excluded from the sales workflow
but remain available for support tracking.

---

## **Working with the action buttons**

When you open a request, a set of gray action buttons appears at the top.
These actions do not modify or save request data. They allow you to:

- Create an email linked to the request
- View all email correspondence
- Import an email manually from your mailbox (emails with the request ticket are imported automatically)
- Print the request
- Copy the request to create a new one using the same data
- View the change history

Hovering over any button shows a **tooltip** explaining its function.

---

## **How to correctly fill out contact name fields**
To maintain record accuracy, CRM provides three separate fields for names:

- First name
- Middle name
- Last name

Only **one word** is allowed in the first and last name fields. If a full name contains more than three words,
all additional words should be placed in the middle name field.
This helps prevent data inconsistency and improves matching accuracy.

---

## **How to avoid duplicate company records**

Pay careful **attention** to the Company name field. Customers often provide shortened or abbreviated company names,
which may cause duplicate company entries.
If the company already exists in the CRM, enter abbreviations and alternate spellings in the "**Alternate Names**"
field of the company profile instead of creating a new company.

---

## **Translation, remarks, and product selection**

- If a request arrives in a foreign language, use the Translation field to provide a translated version.
- This translation will also appear in the deal.
- Enter internal comments or clarifications in the Remark field.
- Use the Products field to select the products or services requested.
  This improves CRM reporting quality and enables product-based filtering in the request list.

---

## **Relationship validation and automatic linking**

When creating a request, Django CRM attempts to find **matching** clients in the database.
If a match is found, the system links the request to an existing lead or  contact and company.
These links appear in the Relationships section, accompanied by a checkbox indicating that the relationships need verification.
Review and confirm these links, and then clear the checkbox once validation is complete.

If no match is found, the CRM will create a **new lead** or contact and company (depending on available data) during deal
creation and automatically link them to the request.

---

## **Viewing email conversations**

The bottom of the request page displays the last four emails exchanged in the conversation.
This gives users immediate context without navigating away from the request.
