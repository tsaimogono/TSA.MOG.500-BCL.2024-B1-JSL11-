# TSA.MOG.500-BCL.2024-B1-JSL11-

# Task Manager Application - ReadMe

# INTRODUCTION 
- This code implements a basic task management application with boards and columns. Users can create tasks, assign them to boards and columns (To Do, Doing, Done), edit them, and delete them.

## Overview
The Task Manager Application helps users manage their tasks efficiently. It allows users to create, edit, and delete tasks, organize tasks into different boards, and switch between different task statuses (such as "To Do", "Doing", and "Done").

## Features
- **Task Creation**: Users can add new tasks with a title, description, and status.
- **Task Editing**: Users can edit existing tasks, including their title, description, and status.
- **Task Deletion**: Users can delete tasks they no longer need.
- **Board Management**: Users can organize tasks into different boards for better organization.
- **Status Filtering**: Users can filter tasks based on their status.
- **Theme Switching**: Users can switch between light and dark themes.

## Code Breakdown

### The code is divided into several sections:

- Imports: Import helper functions from utils and initial data from initialData.js.
- initializeData function: Checks if local storage has data, if not, it loads initial data.
- elements object: Stores references to DOM elements for easier manipulation.
- activeBoard variable: Stores the currently active board name.
- fetchAndDisplayBoardsAndTasks function: Fetches tasks, extracts unique board names, displays boards in the UI, and sets the active board.
- displayBoards function: Creates and displays boards in the DOM.
- filterAndDisplayTasksByBoard function: Filters tasks based on the active board and displays them in their respective columns.
- refreshTasksUI function: Refreshes the task UI by calling filterAndDisplayTasksByBoard with the active board.
- styleActiveBoard function: Styles the active board by adding an active class to the corresponding button.
- addTaskToUI function: Adds a newly created task to the UI within the appropriate column.
- setupEventListeners function: Sets up event listeners for various actions like adding tasks, editing tasks, deleting tasks, toggling sidebar, toggling theme, etc.
- toggleModal function: Shows or hides a modal window.
- addTask function: Handles adding a new task, creates the task object, saves it using createNewTask, and updates the UI.
- toggleSidebar function: Shows or hides the sidebar.
- toggleTheme function: Toggles the application's theme between light and dark based on user preference and stores the setting in local storage.
- openEditTaskModal function: Populates the edit task modal with the task details and sets up event listeners for saving changes and deleting the task.
- saveTaskChanges function: Retrieves updated task information from the edit modal, creates an updated task object, saves it using patchTask, and refreshes the UI.
- init function: Initializes the application by setting up event listeners, checking local storage for sidebar visibility and theme preferences, and fetching and displaying boards and tasks.

## CHALLENGES 
- Error Handling: Used console.log for error handling.
- Complex Data Structures: the complex data structure to manage tasks,boards

## IMPROVEMENTS
- Code Structure: Organize the code into smaller, more manageable functions for better readability and maintainability.
- CSS Styling: Implement CSS styles to improve the application's visual appearance and user experience.
- Responsiveness: Make the application responsive to ensure it adapts to different screen sizes and devices
- Modals: Improve the modal experience by adding animations and transitions.

 ## LEARNING OUTCOMES
 - Syntax: the syntax of the programming language used in the code and understand how to write code correctly.
- Variables: how variables are declared and used. Understanding variables is fundamental because they store data that the program manipulates.
- Conditional Statements: Recognize how conditional statements (like if-else statements) are used to make decisions in the program.
- Loops: Understand how loops (like for or while loops) are employed to iterate over data or perform repetitive tasks.
- Functions: Identify how functions are defined and called.
- Error Handling: learn how to handle errors gracefully.
- Debugging: Analyzing code helped to understand how to debug common issues and errors that arise during development.
- Algorithmic Thinking: Understanding the logic flow of the code helped develop my algorithmic thinking skills.
- Event Listeners:The program demonstrates how to attach event listeners to various UI elements like buttons and forms. These listeners trigger functions when the user interacts with those elements.
- Local Storage:The code utilizes Local Storage to save and retrieve data like the active board, theme preference, and potentially task data (although not implemented in the provided snippet).