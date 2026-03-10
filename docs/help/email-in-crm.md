---
title: Mail in CRM
description: Use Mail in CRM to send, receive, and manage customer emails in one place.
  Improve communication with CRM email management and full CRM with email integration.
---

# Email in CRM

The Mail in CRM page  provides a centralized workspace for managing communication with clients and partners inside
the CRM interface. Instead of switching between multiple tools, users can manage conversations directly within the system,
making Django CRM a practical **CRM with email integration** solution.

With this feature, teams can **send**, **receive**, and **track** **emails** while maintaining full visibility of client communication history.
This approach improves collaboration, ensures consistent communication,
and provides a structured email CRM workflow for customer interactions.

---

## Overview of Email Features

The built-in email system allows teams to handle customer correspondence without leaving the CRM environment.
It combines communication tools with customer and deal management, effectively turning the platform into a **CRM and email** workspace.

Key capabilities include:

- Sending and receiving emails directly from the CRM interface
- Maintaining a centralized correspondence history
- Linking emails automatically to CRM objects such as requests and deals
- Enabling department-level visibility for collaboration

This integrated approach simplifies CRM email management and ensures that all communication remains accessible and organized.

---

## Email Integration and Synchronization

Django CRM supports integration with widely used email providers,
allowing companies to connect their existing mailboxes with the CRM system.

### Supported Email Providers

The platform works with popular email services that support SMTP, including:

- **Gmail**
- **Outlook**
- **Yahoo**
- Other compatible email providers

This makes the platform a flexible CRM with email capabilities that fits into most existing email infrastructures.

### Synchronization with External Email Clients

Users are not required to abandon their preferred email clients. The CRM can synchronize messages with external tools such as:

- Thunderbird
- Outlook
- Other email clients

Emails exchanged through those clients are synchronized with the CRM through the ticket system.

**Important:**

- To **activate** two-way synchronization between the CRM and the connected mailbox,
    at least one email must be sent from the CRM interface first.  
    After activation, correspondence will automatically appear in both systems, ensuring consistent communication records.
- Email synchronization **does not** include **deleting emails**. Rest assured: if you delete emails from your connected
    mailbox (for example, due to exceeding your email provider's storage quota), those emails will remain in your CRM. 
    Your conversation history will be preserved intact.

---

## Automatic Linking to CRM Objects

One of the most valuable **advantages** of the mailing CRM system is automatic context linking.

Every email exchanged with a client is connected to related CRM records, including:

- [Requests](request-processing.md)
- [Deals](deals-management.md)

This means that when users open a request or deal page, they can instantly view the entire email history related to that interaction.

Benefits include:

- Better understanding of client communication history
- Faster issue resolution
- Improved continuity when multiple employees work with the same customer

---

## Viewing Emails in the Mail in CRM Page

The **Mail in CRM** page provides a centralized list of all messages associated with your CRM account.

### Personal Correspondence

Users can view and manage all emails they have exchanged with customers. This includes both sent and received messages,
creating a full communication timeline.

### Department Correspondence

Depending on user permissions, employees can also view the email communication of colleagues within the same department.

- These emails are available in **read-only** mode
- This feature helps team members understand ongoing conversations
- It also supports knowledge sharing and consistent customer service

This transparency is particularly valuable in **collaborative sales** or support teams.

---

## Interface, Sorting, and Navigation

The email list is displayed in a structured table designed for quick navigation and efficient communication management.

Users can organize messages by clicking column headers to sort emails according to:

- **Subject**
- **Sender or Recipient**
- **Responsible user (Owner)**
- **Date sent or received**

Sorting helps users quickly locate the most recent messages or review correspondence related to a particular client.

---

## Searching and Filtering Emails

To simplify navigation within large email volumes, Django CRM provides powerful search and filtering tools.

### Search

Use the search bar to find emails by entering keywords related to:

- Subject lines
- Message content
- Email addresses
- Client names

This feature allows users to locate specific messages within seconds.

### Filters

Filters help narrow down email results based on specific criteria.

Depending on user access permissions, filters may include:

- Mailboxes
- Message owners
- Departments

These filtering options are especially useful for teams that handle a large volume of correspondence
in a shared CRM email management environment.

---

## Creating a New Email

To compose a new message from the CRM interface:

1. Open the **Mail in CRM** page.
2. Click the **Add email** button.
3. Enter the recipient, subject, and message content.
4. If necessary, you can link the email to the corresponding objects.
5. Send the email directly from the CRM.

Once sent, the email will be stored in the CRM.

---

## Benefits of Using Email Inside CRM

Using email directly within the CRM offers several operational advantages:

- Centralized communication history
- Improved collaboration between team members
- Automatic linking of messages to clients, requests, and deals
- Reduced risk of lost or fragmented communication
- Efficient CRM email management for customer relationships

By integrating communication tools with customer data, Django CRM becomes a complete CRM with email integration
platform that supports sales, support, and customer service workflows.

---

## Related Topics

For additional information about email and communication features in Django CRM, see:

- [Email Accounts Management](email-accounts-management.md) – connecting your mailbox to the CRM
- [CRM Email Campaigns](../features/massmail-app-features.md) – sending newsletters and announcements

These guides will help you fully utilize Django CRM as a powerful CRM and email communication platform.
