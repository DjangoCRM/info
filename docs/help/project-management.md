---
title: Project management
description: Overview of the Project List page in Django CRM, including project creation, filtering, sorting, user roles, and stages.
---

# **Project management**

The **Project List** page in [Django CRM](../index.md) allows users to view, filter, and manage all projects created in the system.
A project in CRM is a group of related [tasks](task-management.md) and their subtasks, which together represent a specific goal or activity.
Projects help structure work, monitor progress, and coordinate efforts between team members.

Any CRM user can create and manage projects. Each project has the same attributes and functionality as a task —
you can add tasks to it, track their completion, and monitor the project’s overall progress in real time.

---

## **Creating Projects**

There are several ways to create a project in Django CRM:

- **Direct creation** – click **Add Project** and fill in the project form.
- **From a memo** – create a project directly from an existing [CRM notes](../features/tasks-app-features.md#enhance-your-workflow-with-memos-crm-notes); the form will be automatically filled with the memo’s data.
- **From a task** – convert a task into a project; the project form will inherit the task’s details.

These options make it easy to start a project based on existing CRM records.

---

## **Filtering Projects**

The Project List page includes a filter panel that allows you to narrow down visible projects. You can filter by:

- **Owner (or co-owner)**
- **Assignee (responsible user)**
- **Status** – active or inactive (closed) projects
- **Creation date**

Filters help quickly find relevant projects without searching manually through the entire list.

---

## **Sorting Projects**

Projects are displayed in a structured table with sortable columns. The main columns include:

- **Project name**
- **Next step** – what needs to be done next
- **Next step date** – when it should be completed
- **Completion date** – overall project deadline
- **Priority** – high, medium, or low
- **Stage** – pending, in progress, completed, postponed, or canceled
- **Owners** – project creator(s)
- **Activity status** – active or inactive
- **Project completion date**
- **Project ID**

Most column headers are interactive, allowing users to sort projects by specific parameters. Some fields use icons — hover over an icon to see a tooltip explaining its meaning.

---

## **User Roles in Projects**

Each project in Django CRM includes specific user roles:

- **Project owners and co-owners** – users who create and manage projects.
- **Responsible users** – executors or those assigned to carry out the project.
- **Subscribers** – users who receive notifications about project progress.

Projects are visible only to users involved in them in any of these roles, ensuring data privacy and relevance.

---

## **Project Stages**

Project stages in Django CRM help track progress and keep all participants informed. Available stages include:

- **Pending**
- **In progress**
- **Completed**
- **Postponed**
- **Canceled**

Typically, the **responsible user** updates the project stage, but owners can also make changes. In collective tasks, the first three stages (pending, in progress, completed) are set automatically. Stages can be updated at any time — for instance, if a project marked as “completed” still requires action, the owner can specify a new “next step” and change the stage back to “in progress.”

---

### **Related topics**

* [Task Management in Django CRM](../features/tasks-app-features.md)
* [Creating and Editing Tasks](creating-assigning-tasks.md)
* [Notes CRM – Working with Memos](notes-crm.md)

---

**Notes CRM**: Django CRM provides integrated tools for managing projects, tasks, and memos, helping teams organize work efficiently and maintain full control over ongoing activities.

---
