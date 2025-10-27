---
title: Deleting CRM Memos
description: Learn how to delete CRM notes in Django CRM, including permissions, effects of deletion, and best practices for maintaining organized communication records.
---

# Deleting a CRM Memo

If a [**CRM memo**](../features/tasks-app-features.md#enhance-your-workflow-with-memos-crm-notes) is no longer relevant, you can delete it from the system.
Deleting the note helps keep your workspace organized and ensures that only current
and active communications remain in your CRM.

However, before you proceed with deletion, please review the following important points.

---

## **Who Can Delete a Memo**

Only the **author (owner)** and **recipient** of the memo can delete it.

- Once the recipient reviews the memo and updates its status
  (for example, marks it as *reviewed* or *postponed*),
  the author will no longer be able to delete it.
- If the **recipient** deletes the memo, this is considered bad practice,
  as it can lead to inconsistencies in communication records.

---

## What Happens When a Memo Is Deleted

When you delete a memo, Django CRM carefully removes only the memo
itself without affecting related records.

Please note:

- The list of objects to be deleted may include links between object and users,
  but **users themselves are never deleted**.
- [**Tasks**](../features/tasks-app-features.md) or [**projects**](../features/crm-and-project-management.md) created based on the memo remain in the system.
- **Files** transferred from the memo to a task or project are **not deleted**.

In other words, deleting a memo will not affect other CRM data connected to it — it only removes the note itself.

---

## Related Information

* [Creating a Memo](creating-crm-note.md)
* [Editing a Memo](editing-updating-crm-note.md)
* [Working with CRM Memos](notes-crm.md)

---

## Best Practice

Before deleting a memo, make sure it is no longer needed for reporting, reference, or communication tracking.
If a note contains valuable information related to a project or task, consider leaving it
and marking it as reviewed instead of deleting it.


