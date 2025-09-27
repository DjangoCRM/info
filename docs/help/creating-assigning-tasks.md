---
title: Creating and Assigning Tasks in the CRM
description: Learn how to create, assign, and manage tasks in the CRM to enhance team productivity and collaboration.
---

# **Creating a New Task**

The New Task form in Django CRM helps you quickly create and organize tasks with all necessary details in one place.
You can set a clear title, add a due date, assign responsible employees, define priority, attach files,
and notify team members about progress. Flexible options such as co-owners, subscribers,
and tags make it easier to manage responsibilities and keep everyone informed.
Below is an explanation of each field in the form and how it works.

---

## **Task Details**

- **Name**  
  Enter the title of the task. This is a required field and should clearly describe the purpose of the task.

- **Due date** *(optional)*  
  If needed, select a deadline using the built-in calendar.
  You can leave this field empty if the task has no strict completion date.
  If an error occurs when manually entering a date, use the calendar to see what format the data should be in.

- **Priority**  
  Choose the importance of the task:

    - **Low** – non-urgent or routine work.
    - **Middle** – standard priority (selected by default).
    - **High** – urgent or business-critical task.

- **Description** *(optional)*  
  Provide additional details about the task. This field can be used to explain the scope, goals, or specific requirements.

- **Note** *(optional)*  
  Add short remarks, internal comments, or reminders related to the task.

---

## Assignment

- **Responsible**  
  The performer(s) of the task. By default, you are automatically selected.

    - If you are a department manager, you can also assign the task to members of your team.
    - If you are the head of the company, you will see a full list of all employees added to the CRM.

- **Owner**  
  You are automatically assigned as the task owner. This field cannot be changed.

  - **Co-owner**  *(optional)*  
  Assign a co-owner to the task. This person will share responsibility for overseeing the task's progress and completion.
  The co-owner will have the right to change the task.  
  The system will suggest a co-owner automatically:

    - If you are a regular employee, your department head will be proposed.
    - If you are a department head, the company head will be proposed.
    - If you are the company head, no co-owner will be suggested.

  You can leave this field empty if you do not want to assign a co-owner.

  - **Change Subscribers** *(drop-down section)*  
  Select users who should be notified about the task and its progress.
  Subscribers do not perform the work but stay informed about updates and results.
  When creating a subtask, the system automatically selects the other assignees of the main task.
  You may remove any of them if necessary.

- **Add Tags** *(drop-down section)*  
  Assign one or more tags to the task for easier categorization and searching later.
---

## **Attachments**

- **Files**
  Upload and attach files to the task. These may include documents, spreadsheets,
  or other materials that will help in completing the work.

---

## **Notifications and Access**

After saving a task, all users selected in it will receive a notification appropriate to their role.
The task will become available in their [task manager](task-management.md).
Other users (except your managers and administrators) will not have access to it.

---

## **Additional Resources**
For more information on task management features and best practices, refer to the following resources:
- [Task Management Features](../features/tasks-app-features.md)
- Project Management
- Memos in CRM

---
## **Summary**

By filling out the **New Task** form, you can set deadlines, assign responsible people, notify the right colleagues,
and provide all the necessary information in one place. This ensures that tasks are clearly structured and
progress can be tracked effectively in the CRM.
This leads to better team collaboration and higher productivity.