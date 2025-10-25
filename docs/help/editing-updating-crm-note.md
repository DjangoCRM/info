---
title:  Editing and Updating CRM Memos
description: Learn how to edit and update CRM memos in Django CRM, including permissions, status updates, and integration with tasks and projects.
---

# **Editing and Updating CRM Memos**

Django CRM allows users to edit or update existing [memos](notes-crm.md) — CRM notes — while maintaining
full transparency over who made changes and when. A memo can be edited only by its **owner (author)**
or **recipient**, ensuring controlled access and accountability.

---

## **Who Can Edit a Memo**

* **The owner (author)** can edit or delete the CRM memo while its status is **Pending**.
* **The recipient** can update the memo’s status to **Reviewed** or **Postponed**. Once the recipient changes the status, the author loses the ability to edit or delete the memo.

The **"Modified By"** field displays the name of the last user who edited the memo, and you can view the **entire edit history** by clicking the **History** button.

---

## **Forwarding and Status Updates**

Recipients can **forward a memo** to another user by selecting a new recipient. This allows the memo to move through the appropriate approval or review chain.

Changing a memo’s status helps track progress and ensure that each note receives timely attention.

---

## **Creating a Task or Project as a result of reviewing the Memo**

The recipient can **[create a task](creating-assigning-tasks.md) or project** directly from a memo. In this case:

* All memo data, including attached files, will be automatically transferred.
* The memo’s **author and subscribers** will become **subscribers to the new task or project** and will receive notifications.
* The recipient can add their own notes or conclusions in the **“Conclusion”** field.

If a task or project has been created, a **button to view it** will appear in the memo.

> Learn more: [CRM and Task Management](../features/tasks-app-features.md) | [CRM and Project Management](../features/crm-and-project-management.md)

---

## **Creating Reminders or New Memos**

You can easily create a **reminder** or a **new note** based on the current memo by clicking the **Copy** button. This simplifies repetitive documentation and helps track related activities.

> Related topic: [Memo creation](creating-crm-note.md)

---

## **Using the Built-in Chat**

Every memo has a **built-in chat** where users can discuss its contents and coordinate updates.

* The **author** can use the chat to comment or provide updates after the memo is reviewed (since direct editing will no longer be available).
* If a **task or project** has been created based on the memo, further discussions should continue in the corresponding **task or project chat**.

---

## **Additional Options**

If the memo was originally created from a **deal**, a **“View deal”** button will appear, allowing you to quickly navigate to the associated CRM record.

> Related topic: Working with Deals in CRM

---

By providing structured permissions, detailed history tracking, and integration with tasks,
projects, and chats, Django CRM ensures that memo management remains transparent and efficient.
