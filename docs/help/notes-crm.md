---
title: Working with Memos (CRM Notes)
description: Learn how to use the Django CRM memo list to view, sort, and filter CRM notes, manage internal memos, and track related tasks.
---

# **Working with Memos in Django CRM**

Notes CRM provides users with convenient functionality for working with **memos (CRM notes)** —
internal messages that can serve as personal notes, office memos, or
service notes. Any CRM user can create a memo and specify who it is intended for:
themselves, their department manager, or the company.

Memos allow users to document internal communications and keep all related information within the Notes CRM module.
This feature helps teams maintain a structured record of communications, decisions, and follow-up actions.

---

## **User Roles in CRM Memos**

Each memo has several user roles that define how participants interact with it:

- **Owners** – users who create CRM memos.
- **Recipients** – those for whom the memos are intended.
- **Subscribers** – users who should be notified about the memo and, if applicable, about tasks created as a result of reviewing it.

---

## **Memo Stages**

The following stages are available for informing participants:

- **Pending** – memo is awaiting consideration.
- **Postponed** – review is delayed.
- **Considered** – memo has been reviewed.

The stage of a CRM memo is updated by its recipient.
After the stage **“considered”** is set, the owner can no longer edit it or change
attached files.

All participants are automatically notified in the CRM interface and by email when a memo is created or reviewed.
The same notification method applies to messages in the memo chat.

---

## **Memo Chat and Related Tasks**

Each memo includes a **chat** where participants can exchange messages and files.
For example, users can clarify details or notify others about follow-up actions after reviewing the memo.  
If a task is created as a result of reviewing the memo, further communication should take place in the **task chat** instead.

In the memo list, a **“View task”** button appears next to memos that resulted in a task.
The **button color** indicates the task stage, and the **tooltip** shows the stage name when hovering over it.

The integration between memos and tasks in **Notes CRM** ensures that decisions and actions stay connected, allowing users to trace every step from communication to execution.

---

## **Memo List Overview**

The **memo list page** is the central workspace for managing all CRM notes.
Here, users can view, sort, filter, and search memos, as well as create new ones or duplicate existing ones.

Memos are displayed in a table containing the following information:

- **Memo title**
- **Recipient** (to whom the memo is intended)
- **File icon** (indicates attachments)
- **Status icon** (a tooltip appears when hovering over it)
- **Date reviewed** (when the recipient reviewed the memo)
- **Open task button** — appears if a task was created after the memo review; its color corresponds to the task stage (a tooltip appears when hovering over it)
- **Memo owner (author)**
- **Owner’s department**
- **Creation date**
- **Copy memo button** – opens a new memo form pre-filled with the current memo’s data

---

## **Sorting, Filtering, and Searching**

Users can easily navigate through memos using built-in tools:

- **Sorting** – by title, recipient, author, and creation date.
- **Filtering** – by stage, recipient, owner, or creation date.
- **Search** – by keyword or memo ID.

Each user sees only those memos where they are listed in any role (owner, recipient, subscriber).

---

## **See Also**

For more details on how to create or manage memos, see related help topics:

- [Creating a Memo in Django CRM](creating-crm-note.md)
- [Editing and Reviewing Memos](editing-updating-crm-note.md)
- [CRM notes and Tasks](../features/tasks-app-features.md)

---

## **Notes CRM**

Using the memo functionality in Django CRM helps organize internal communication and preserve important work-related information within the system.
With **Notes CRM**, users can efficiently create, share, and review memos, attach supporting files, and link discussions to actionable tasks.
This functionality makes Django CRM a practical solution for managing both day-to-day notes and formal business correspondence in one place.
