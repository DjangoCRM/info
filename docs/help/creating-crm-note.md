---
title: Creating a Memo in the CRM
description: Learn how to create and manage memos (CRM notes) in Django CRM to enhance internal communication and organization.
---

# **Creating a Memo - CRM note**

The **Memo creation page** in Django CRM allows users to create and send internal memos — personal notes,
office memos, or service notes — to themselves, managers, or the entire company.
This function helps organize communication within the CRM, record decisions,
and [initiate task](task-management.md) resulting from the memo review.

---

## **Who Can Create a Memo**

Any CRM user can create a memo. The author of a memo is its **owner** and has full control over its contents until it is reviewed.
Once the memo is reviewed and its status changes to *considered*, the owner can no longer edit or replace files attached to it.

---

## **Memo Roles**

When creating a memo, users define its participants:

- **Owner** – the user who creates the memo (assigned automatically).
- **Recipient** – the user for whom the memo is intended (selected from the available list).
- **Subscribers** – users who should be informed about the memo (they receive notifications and can view the memo).

---

## **Memo Statuses and Stages**

When you create a memo, you can first save it as a **draft**.
In this case, only you (and CRM administrators) can see it, and no notifications are sent.

After a memo is shared with other users, it goes through several **stages**:

- **Pending** – the memo awaits review.
- **Postponed** – review has been delayed.
- **Considered** – the memo has been reviewed. At this stage, the memo content becomes locked for editing.

All participants receive CRM and email notifications when the memo is created and when its status changes.

---

## **How to Create a Memo**

To create a new memo, go to the [**Memo list page**](notes-crm.md) and click **ADD MEMO** or **Copy note** icone.
The second option opens a pre-filled form based on the selected memo’s data.

Fill in the memo creation form fields:

1. **Memo title** – enter a short, clear name for the memo.
2. **Draft checkbox** – select if you want to save the memo as a draft (visible only to you).
3. **Recipient** – choose the user the memo is intended for.
4. **Purpose (optional)** – choose one of the predefined purposes:

    - for information
    - for consideration
    - on approval
    - for the record
    - to make a decision
    - payment of regular expenses

5. **Description** – provide detailed content of the memo.
6. **Subscribers** – select users who should be notified about the memo.
7. **Attachments** – upload files related to the memo.

Once you save the CRM note, it will appear in your **Memo list** and
become visible to all users specified in it (recipients and subscribers).
They will also receive automatic notifications about its creation.

---

## **Related Pages**

- [Memo list page](notes-crm.md) – view, search, and manage your memos.
- [Memo editing page](editing-updating-crm-note.md) – update an existing memo before it’s reviewed.
- [Memo deletion page](deleting-crm-note.md) – confirm and delete a memo if necessary.

---

**Tip:** Use memos not only as reminders but also as a formal way to document decisions, internal approvals,
and actions that require follow-up tasks.

