# React.js Mini Project Assignment

## Project Title: Task Manager Web App

## Objective
The goal of this assignment is to build a **Task Manager Application using React.js** where users can create, update, delete, and manage their daily tasks.

This project will help students practice:
- React Components
- React Hooks (useState, useEffect)
- Props and State management
- Form handling
- Conditional rendering
- Local storage usage
- Basic UI styling

---

# Project Description

You need to build a **Task Manager Web Application** where users can:

- Add new tasks
- Edit existing tasks
- Mark tasks as completed
- Delete tasks
- Filter tasks (All / Completed / Pending)

All tasks should be **saved in browser local storage** so that tasks remain after page refresh.

---

# Required Features

## 1. Add New Task

Users should be able to add a task using an input form.

Task fields:

- Task Title
- Task Description
- Due Date

Example:

Title: Complete React Assignment  
Description: Finish React mini project  
Due Date: 20 June 2026

When user clicks **Add Task**, the task should be added to the list.

---

# 2. Display Task List

All tasks should be displayed in a list or card format.

Each task card should display:

- Task Title
- Description
- Due Date
- Status (Completed / Pending)

Example:

Task: Complete React Assignment  
Description: Finish React mini project  
Due Date: 20 June  
Status: Pending

---

# 3. Mark Task as Completed

Each task should have a **checkbox or button** to mark it as completed.

When completed:

- Task status should update
- UI should visually show completion (like strikethrough text)

---

# 4. Edit Task

User should be able to edit task details.

Workflow:

1. Click **Edit button**
2. Open edit form
3. Update task information
4. Save changes

---

# 5. Delete Task

Each task should have a **Delete button**.

When clicked:

- Remove task from the list
- Update local storage

---

# 6. Task Filtering

Add filter buttons:

- All Tasks
- Completed Tasks
- Pending Tasks

Behavior:

| Filter | Result |
|------|------|
| All | Show all tasks |
| Completed | Show completed tasks |
| Pending | Show incomplete tasks |

---

# 7. Local Storage Integration

Tasks should be stored in **browser local storage**.

Example:

```javascript
localStorage.setItem("tasks", JSON.stringify(tasks))
