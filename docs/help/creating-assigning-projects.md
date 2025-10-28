---
title: Creating and Assigning Projects
description: Learn how to create and assign projects in Django CRM, including setting priorities, deadlines, and responsible users.
---

# **Creating a Project in CRM**

When working with projects in [**Django CRM**](../index.md), users can easily create new projects
and assign responsibilities, priorities, and deadlines. Each project groups related [tasks](task-management.md)
and provides a structured way to manage workflows across departments or teams.

---

## **Fields in the Project Creation Form**

Each field in the form helps define how the project will be [managed](project-management.md) and who will be involved:

- **Name** — Enter the title of the project.
  This is a required field and will appear in the project list.

- **Due date** *(optional)* — Set a completion date for the project.
  You can select the date directly from the built-in calendar.

- **Priority** — Choose the priority level for the project:
  **Low**, **Middle**, or **High**. The system suggests **Middle** by default.

- **Description** *(optional)* — Add a short description of the project’s purpose,
  scope, or goals.

- **Note** *(optional)* — Use this field for additional comments or internal remarks.

- **Responsible** — Specify the users who will be responsible for executing the project tasks.

- **Owner** — The user who creates the project is automatically assigned as its owner.

- **Co-owner** *(optional)* — You can add another user as a co-owner to share management rights.

---

## **Optional Sections**

Below the main fields, the form contains several expandable sections for
additional configuration:

- **Change Subscribers** — Select users who should receive notifications about project
  updates and progress. This helps keep relevant team members informed without
  assigning them as performers.

- **Add Tags** *(optional)* — Tags make it easier to categorize projects and quickly
  filter them in the project list.

- **Files** — Attach files directly to the project. This can include project briefs,
  specifications, reports, or any supporting documentation.

---

## **Saving the Project**

After completing all required fields, click **Save** to create the project.
The new project will appear in your **Project List** or click **Save and Continue**
to start adding tasks to the project.

> [Working with Tasks in Django CRM](../features/tasks-app-features.md)
