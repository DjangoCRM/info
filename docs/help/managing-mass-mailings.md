---
title: Managing Mass Mailings
description: Learn how to manage mass mailings in mailing CRM, including creating mailings, monitoring progress,
  handling errors, searching, filtering, and combining mailings.
---

# **Managing Mass Mailings in Django CRM**

The **Mass Mailing software** module in Django CRM helps sales and marketing teams manage company newsletters,
product updates and promotional messages using the built-in [**mailing CRM**](../index.md) tools.
This section describes how to create, monitor their progress, and optimize **mass mailing** campaigns,
ensuring efficient and compliant [**email marketing**](../features/massmail-app-features.md) workflows.

Mass mailings can be sent to **companies**, **contacts**, or **leads**. All recipients come directly from your
CRM database, ensuring clean segmentation and accurate targeting—key elements of successful email marketing.

---

## **Key Features of the CRM Mass Mailing Tool**

The mailing CRM module offers multiple built-in features that support efficient and secure delivery:

- Email newsletters are sent through sales managers’ email accounts.
- The system includes a built-in unsubscribe mechanism. Recipients may **unsubscribe** at any time.
- Protect email accounts from spam-blocking mechanisms through automatic sending limits and scheduling rules.
- Each email account has a **daily sending limit**, and emails are sent **evenly throughout working hours**.
- Mass mailings are automatically suspended on Fridays, Saturdays, and Sundays.
- Main sales manager email accounts send newsletters only to **VIP recipients**, reducing spam risks.

These safeguards maintain a good sender reputation and improve overall email marketing performance.

Each mailing operation is stored as a Mailing object, which contains:

* Initial configuration of the mass mailing
* Ongoing sending progress
* Final results when the mailing is completed

---

## **Creating a New Mass Mailing**

Before creating a mailing, ensure you have:

- At least **one configured email account** for sending newsletters.
- A **newsletter template** is created and ready.
- An email **signature** is prepared (recommended).

You can create a new mailing in several ways:

1. On the main **Mass Mailing** page by clicking **Make Massmail**.
2. From the [**Lead**](lead-management.md), [**Company**](company-management.md),
   or [**Contact**](contact-management.md) pages—each object type has the option to initiate a Massmail.

A separate mailing is created **per recipient type** (leads, companies, or contacts).
Sales managers can only create mailings for recipients assigned to them.

### Access Permissions

Access depends on role and department:

* **Sales managers** see only mailings from their own department.
* **Company managers** see mailings from **all** departments.

<!-- For more on permissions, see: ➡️ *[Managing Departments in CRM](#)* ➡️ *[User Roles and Access Rights](#)* -->

---

## **Mass Mailing List Overview**

The mass mailing list appears in a sortable, filterable table, allowing teams to quickly analyze campaign data.

### Table Columns

- Name and newsletter preview
- Recipient type (leads, companies, contacts)
- Status
- Completion percentage
- Assigned sales manager
- Emails sent today
- Number of recipients
- Number of available email accounts
- Notifications and error messages

Email accounts assigned to a sales manager are represented by green and red stars.
<?xml version="1.0" encoding="utf-8"?>
<svg width="15px" height="15px" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill="#379634" d="M10 15l-5.878 3.09 1.123-6.545L.489 6.91l6.572-.955L10 0l2.939 5.955 6.572.955-4.756 4.635 1.123 6.545z"/></svg><?xml version="1.0" encoding="utf-8"?>
<svg width="15px" height="15px" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill="#379634" d="M10 15l-5.878 3.09 1.123-6.545L.489 6.91l6.572-.955L10 0l2.939 5.955 6.572.955-4.756 4.635 1.123 6.545z"/></svg><?xml version="1.0" encoding="utf-8"?>
<svg width="15px" height="15px" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill="#e4572e" d="M10 15l-5.878 3.09 1.123-6.545L.489 6.91l6.572-.955L10 0l2.939 5.955 6.572.955-4.756 4.635 1.123 6.545z"/></svg>  
A green account color indicates that this account can be used for sending emails.

### Mailing Statuses

Mailings may have the following statuses:

* **Active** – sending is in progress
* **Active but error** – sending continues but issues occurred
* **Paused**
* **Interrupted** – sending stopped due to critical errors
* **Done** – mailing completed

To display the latest data, refresh the page. When launching a new mailing, progress details will appear within approximately **5 minutes**.

---

## **Handling Errors During Mass Mailing**

If an error occurs:

- The status updates to **Active but error**.
- A detailed message appears in the **Notifications** column.
- For multiple errors, the field becomes scrollable.
- Critical errors stop the newsletter with an Interrupted status

If some recipients did not receive the email:

1. Resolve the reported issues (e.g., email account limit, invalid addresses).
2. Restart the mailing for **only the unsuccessful recipients** on the mailing details page.

---

## **Searching and Filtering Mass Mailings**

Use the search bar to find mailings by:

- Keywords (e.g., mailing name)
- Mailing ID

Available filters include:

- Department (if user role allows)
- VIP status
- Owner - assigned sales manager

These filters allow you to quickly navigate large volumes of mailings.

---

## **Combining Multiple Mailings**

The Action menu allows you to merge multiple mass mailings into a single one.
Mailings can be combined only when they have:

- The same newsletter message
- The same recipient type
- Mailing owner (sales manager)

This feature helps avoid duplicated email marketing campaigns and simplifies workflow management.
