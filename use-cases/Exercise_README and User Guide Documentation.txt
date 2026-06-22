Project Information Chosen

Project Name: Task Manager

Description: A Java-based task management system that allows users to create, update, organize, prioritize, and track tasks.

Key Features:

Create and manage tasks
Set task priorities
Assign due dates
Track task status
Add and remove tags
View overdue tasks
Generate task statistics
Store tasks in JSON format

Technologies Used:

Java
Gson
JSON Storage
LocalDateTime API
Prompt 1: Comprehensive README
Task Manager
Description

Task Manager is a Java application designed to help users create, organize, and track tasks efficiently. The system supports task 
prioritization, due dates, status tracking, tagging, overdue task monitoring, and statistical reporting.

Features
Create new tasks
Update task details
Delete tasks
Assign priorities
Set due dates
Add tags
Mark tasks as completed
Track overdue tasks
Generate task statistics
Save data in JSON format
Technologies Used
Java
Gson Library
JSON File Storage
Java Collections Framework
LocalDateTime API
Installation
Prerequisites
Java JDK 8 or higher
IDE such as VS Code or IntelliJ IDEA
Steps
Clone or download the project.
Open the project in your IDE.
Add the Gson library dependency.
Build the project.
Run the application.
Basic Usage
Create a Task
Task task = new Task(
    "Complete Assignment",
    "Finish Java project",
    TaskPriority.HIGH,
    dueDate,
    tags
);
List Tasks
taskManager.listTasks(null, null, false);
Mark Task as Done
task.markAsDone();
Configuration

The system stores task information in a JSON file specified when creating the TaskManager object.

Example:

TaskManager manager = new TaskManager("tasks.json");
Troubleshooting
Tasks Not Saving

Verify the JSON file location is valid and writable.

Invalid Date Error

Use the format:

YYYY-MM-DD

Example:

2026-06-30
Gson Errors

Ensure the Gson library is included in the project dependencies.

Contributing
Fork the repository.
Create a new branch.
Make your changes.
Commit your updates.
Submit a pull request.
License

This project is licensed under the MIT License.

Prompt 2: Step-by-Step Guide
How to Create and Manage a Task
Prerequisites
Java installed
Task Manager application running
Step 1: Create a Task

Provide:

Title
Description
Priority
Due Date
Tags

Example:

manager.createTask(
    "Assignment",
    "Complete Java documentation",
    3,
    "2026-06-30",
    List.of("school", "java")
);
Step 2: View Tasks.

Display all tasks:

manager.listTasks(null, null, false);
Step 3: Update Task Priority
manager.updateTaskPriority(taskId, 4);

This changes the priority to URGENT.

Step 4: Update Task Status
manager.updateTaskStatus(taskId, "done");

The task will automatically be marked as completed.

Step 5: Add Tags
manager.addTagToTask(taskId, "important");
Step 6: Check Overdue Tasks
manager.listTasks(null, null, true);
Troubleshooting
Task Not Found

Verify the task ID exists.

Invalid Status

Use:

todo
in_progress
review
done
Invalid Priority

Use:

1 = LOW
2 = MEDIUM
3 = HIGH
4 = URGENT
Prompt 3: FAQ Document
Frequently Asked Questions (FAQ)
What is Task Manager?

Task Manager is a Java application used to create, organize, and track tasks.

How do I create a task?

Use the createTask() method and provide the required information such as title, description, priority, and due date.

How do I change task status?

Use:

updateTaskStatus(taskId, "done");
How do I set task priorities?

Priority values are:

Value	Priority
1	LOW
2	MEDIUM
3	HIGH
4	URGENT
How do I add tags?

Use:

addTagToTask(taskId, "important");
How do I view overdue tasks?

Use:

listTasks(null, null, true);
Where are tasks stored?

Tasks are stored in a JSON file.

What date format should I use?

Use:

YYYY-MM-DD

Example:

2026-06-30
What happens when a task is completed?

The status changes to DONE and the completion date is recorded automatically.

What should I do if tasks are not saving?

Check that:

The JSON file path is correct.
The application has write permissions.
Gson is correctly configured.
Reflection
Which aspects of the project were most challenging to document?

The task management workflow and the interaction between task status, priorities, due dates, and statistics were the most 
challenging parts to document.

How did you adjust your prompts to get better results?

I provided information about the project structure, features, technologies used, and expected documentation sections to generate 
more accurate documentation.

What did you learn about document structure and organization?

Good documentation should include installation instructions, feature descriptions, usage examples, troubleshooting information, 
and FAQs to help users understand the system.

How would you incorporate this approach into your development workflow?

I would use AI-generated documentation to quickly create README files, user guides, and FAQs while developing software projects, 
then review and refine the output before publishing.