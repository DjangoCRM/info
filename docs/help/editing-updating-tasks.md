---
title: Editing and Updating Tasks in the CRM
description: Learn how to edit and update tasks in the CRM to enhance team productivity and collaboration.
---

# **Editing and Updating Tasks**

The task editing form in Django CRM helps you update task details, track progress, and collaborate with colleagues.
You can change the task stage, define the next step with a deadline, set reminders, and view workflow history.
Additional options such as creating subtasks, chatting with participants, copying tasks,
or checking task history make task management flexible and transparent for both individual users and teams.  
Below is an explanation of the new fields and buttons available in the task editing form.  
For a general overview of how tasks are organized, read about the [CRM Task Management](../features/tasks-app-features.md).

---

## **Additional Fields in the Task Editing Form**

- **Stage**  
  Defines the current status of the task. Available values are:

    - **Pending** *(default)* – task is created but not yet started.
    - **In progress** – task is actively being worked on.
    - **Done** – task is completed.
    - **Postponed** – task is delayed for later.
    - **Canceled** – task will not be completed.

- **Next step**  
  Specifies the next action required for the task.
  The value entered here is also displayed in the user’s task list, helping participants understand what to do next.

- **Next step date**  
  Defines the planned date for the next step. This date is displayed in the task list so users can see upcoming deadlines.

- **Remind me** *(checkbox)*  
  When enabled, the CRM automatically creates a reminder and sends it to the user on the **Next step date**.

- **Hide the main task** *(checkbox in subtasks)*
  Allows you to hide the primary task in your [CRM task manager](task-management.md) before it's completed by all assignees.

- **Workflow**  
  This field is filled automatically by the CRM whenever the **Next step** field changes.
  It records what actions were taken and when, forming a history of task progress.

Other fields are described in detail in the [Creating a New Task](creating-assigning-tasks.md) section.

---

## **New Buttons in the Task Editing Form**

- **Create subtask**  
  Allows you to create a subtask linked to the current task.

- **Add message to chat of this task**  
  Opens the chat for this task, where all task participants, managers, and operators (if assigned)
  can exchange messages and files. Each task and subtask has its own separate chat.

- **Chat**  
  Appears when there is at least one message in the task chat. Use it to view the full conversation history and reply.
  Tasks with chat messages are marked with an icon in the [task manager](task-management.md).
  The icon changes color if there are unread messages for you in the chat.

- **Subtasks** *(with counter)*  
  Displays a list of all subtasks associated with the main task, accessible to all participants.

- **View main task** *(in subtasks)*  
  Appears in the subtask editing form. Click it to return to the main task.

- **Copy**  
  Creates a new task based on the current one. The task creation form will open with all fields pre-filled from
  the existing task, which you can adjust before saving.

- **Create reminder**  
  Lets any participant create a personal reminder for the task. The button changes color when at least one reminder exists.

- **History**  
  Opens the task history log, showing all changes made, who made them, and when.

---

## **Special Button for Team Tasks**

- **Completed**  
  Appears in tasks assigned to a team. When clicked, the CRM automatically creates a subtask for the user
  and immediately marks it as completed. All team members are notified of this action.

---

## **Summary**

By updating tasks in the [CRM with task management](../features/tasks-app-features.md), users can set clear stages, define next steps with deadlines,
use reminders, and communicate directly in task chats. Additional buttons make it easier to manage subtasks,
track history, and copy existing tasks.
This ensures that teamwork remains transparent and organized at every stage of task execution.

