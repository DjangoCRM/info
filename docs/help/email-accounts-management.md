---
title: Email Accounts Management
description: Learn how to manage email accounts in Django CRM, including viewing account details,
  monitoring synchronization status, and understanding the main account logic for CRM mailing and mass mailing campaigns.
---

# Email Accounts Page in Django CRM

The **Email Accounts** page in Django CRM is the control center for configuring and monitoring all
email channels used for client communication, CRM mailing, and CRM email marketing campaigns.

Django CRM supports integration with any email provider that works via SMTP and IMAP protocols,
including services such as **Gmail**.
This enables reliable two-way synchronization for both individual correspondence and large-scale mass mailing operations.

---

## What You Can See on the Email Accounts Page

All connected and assigned email accounts are displayed in a structured table.
This overview provides operational transparency for your CRM mailing and mass mail activities.

The table allows you to quickly identify:

- **Accounts assigned to you**
  A complete list of email accounts you are authorized to use.

- **Default account for customer communication**
  The account currently designated by the CRM as the primary one for outgoing correspondence.

- **Automatic synchronization status**
  Indicates which accounts have IMAP synchronization enabled.
  This is especially important for importing incoming emails that contain tickets and automatically linking them to CRM records.

- **Daily sending activity**

    - Timestamp of the last email sent
    - Total number of emails sent on that day through each account
      This helps you monitor workload distribution and detect unusual activity during mass mail campaigns.

- **System notifications**
  CRM displays notifications related to:

    - Errors during a mass mailing or CRM email marketing campaign
    - Successful completion of a mailing campaign

This operational visibility allows you to assess performance and reliability of each account used for CRM mailing.

---

## Viewing Detailed Account Information

To access extended information, click on a specific email account in the list.

The detailed view may include:

- Login credentials (visible depending on permissions)
- SMTP and IMAP configuration parameters
- Synchronization settings
- Account usage statistics

This section is particularly useful when troubleshooting issues related to mass mail,
CRM email marketing campaigns, or email import errors.

---

## Important Configuration Notes

### 1. Administrative Access Required

Correct configuration of SMTP and IMAP parameters requires technical expertise.
If you need to modify email account settings, contact your CRM administrator.

Improper configuration may lead to:

- Failed CRM mailing campaigns
- Broken synchronization
- Email delivery errors
- Incomplete ticket imports

---

### 2. Main Account and VIP Logic

Django CRM applies a specific rule for the **main email account**:

- The main account is used for sending mailings **only to recipients marked as VIP**.
- If your selected audience for a mass mailing contains no VIP contacts, emails will **not** be sent
  through the main account — even if it is authorized for use in CRM email marketing.

This rule ensures priority handling of strategic clients and prevents misuse of primary communication channels.

---

## Best Practices for CRM Mailing and Mass Mailing

To ensure stable CRM email marketing operations:

- Regularly monitor sending statistics for each account.
- Verify synchronization status for accounts responsible for ticket processing.
- Check CRM notifications after every mass mail campaign.
- Coordinate with your administrator before modifying account settings.
- Confirm VIP tagging before launching a campaign that depends on the main account.

---

## Related Topics

For more information, see:

- [Mass Mailing Management](managing-mass-mailings.md) – How to create and launch a mass mailing campaign in CRM
- [Managing Company Contacts](contact-management.md) – How VIP status affects CRM mailing logic

---

The Email Accounts page is a critical operational module in Django CRM.
Properly configured accounts ensure reliable CRM mailing, accurate ticket synchronization,
and effective CRM email marketing performance.
