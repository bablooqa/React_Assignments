
# React.js Mini Project Assignment

## Project Title
**Task Manager Web Application**

---

# Objective

The goal of this assignment is to build a **Task Manager Web Application using React.js**.  
Students will create an application where users can manage daily tasks such as creating, updating, completing, and deleting tasks.

This project will help students learn and practice:

- React project structure
- Functional components
- React Hooks (useState, useEffect)
- Props and component communication
- CRUD operations
- Conditional rendering
- Working with browser localStorage
- UI structuring

---

# Project Overview

Students need to build a **Task Manager application** where users can:

- Add tasks
- Edit tasks
- Delete tasks
- Mark tasks as completed
- Filter tasks (All / Completed / Pending)
- Save tasks in local storage so data persists after refresh

---

# Technologies to Use

Students should use:

- React.js
- JavaScript (ES6+)
- HTML
- CSS / Bootstrap / Tailwind (optional)

---

# Functional Requirements

## 1. Add New Task

Users should be able to create a new task using a form.

The form should include:

- Task Title
- Task Description
- Due Date

Example:

Title: Complete React Assignment  
Description: Build task manager mini project  
Due Date: 20 June 2026

When the **Add Task** button is clicked:

- Task should be added to the task list
- Input fields should reset

---

# 2. Display Task List

All tasks should appear on the screen.

Each task card should display:

- Task Title
- Task Description
- Due Date
- Task Status

Example:

Task: Complete React Assignment  
Description: Build task manager mini project  
Due Date: 20 June  
Status: Pending

---

# 3. Mark Task as Completed

Each task should include:

- Checkbox OR
- Complete button

When clicked:

- Task status should change to **Completed**
- UI should show completed style (example: strike-through text)

Example:

~~Complete React Assignment~~

---

# 4. Edit Task

Users must be able to update task information.

Workflow:

1. Click **Edit**
2. Open editable form
3. Update details
4. Click **Save**
5. Task updates in list

---

# 5. Delete Task

Each task must include a **Delete button**.

When clicked:

- Remove task from the list
- Update local storage

---

# 6. Task Filters

Students should implement filter buttons.

Filters:

- All Tasks
- Completed Tasks
- Pending Tasks

Expected Behavior:

| Filter | Result |
|------|------|
| All | Show all tasks |
| Completed | Show completed tasks |
| Pending | Show incomplete tasks |

---

# 7. Local Storage Integration

Tasks must be stored in **browser localStorage**.

Example:

```javascript
localStorage.setItem("tasks", JSON.stringify(tasks))
```

Load tasks on page load using:

```javascript
useEffect(() => {
  const storedTasks = JSON.parse(localStorage.getItem("tasks")) || []
  setTasks(storedTasks)
}, [])
```

---

# UI Requirements

The interface should be clean and simple.

Students may use:

- Basic CSS
- Bootstrap
- Tailwind CSS

Suggested Layout:

-----------------------------------
Task Manager
-----------------------------------

Add Task Form

Title: ____________
Description: _______
Due Date: _________

[ Add Task ]

-----------------------------------

Filters:
[All] [Completed] [Pending]

-----------------------------------

Task List

[ ] Task Title  
Edit | Delete

[✓] Completed Task  
Edit | Delete

---

# Suggested Folder Structure

task-manager-app

public/

src/
components/
TaskForm.js  
TaskList.js  
TaskItem.js  
FilterButtons.js  

App.js  
App.css  
index.js  

package.json

---

# Required React Concepts

## Functional Components

Example:

```javascript
function TaskItem() {
  return <div>Task</div>
}
```

---

## React Hooks

### useState

```javascript
const [tasks, setTasks] = useState([])
```

### useEffect

Used for loading tasks from local storage.

---

## Props

Example:

```javascript
<TaskList tasks={tasks} />
```

---

# Optional Bonus Features

Students can add:

- Search tasks
- Task priority (High / Medium / Low)
- Dark mode
- Drag & drop tasks
- Task categories
- Mobile responsive UI

---
