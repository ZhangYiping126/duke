# User Guide

## User Inteface
![alt text][screenshot]

[screenshot]: Ui.png 

## Features 

### 1. Adding a todo task: `todo` 

Adds a todo task to the task list.

Format: `todo DESCRIPTION`

Example of usage: 

`todo do assignment`

Expected outcome:
```
Got it. I've added this task:
   [T][✘] do assignment
Now you have 1 task in the list.
```

### 2. Adding a deadline task: `deadline` 

Adds a deadline task to the task list. 
The date follows `yyyy/MM/dd` format 

Format: `deadline DESCRIPTION /by DATE`

Example of usage: 

`deadline have fun /by 2020-06-01`

Expected outcome:
```
Got it. I've added this task:
  [D][✘] have fun (by: June 1 2020)
Now you have 2 tasks in the list.
```

### 3. Adding a event task: `event` 

Adds a event task to the task list. All the dates follows 
`yyyy/MM/dd` format

Format 1: `event DESCRIPTION /at DATE`

Example of usage: 

`event attend conference /at 2020-01-01`

Expected outcome:

```
Got it. I've added this task:
  [E][✘] attend conference (at: Jan 1 2020)
Now you have 3 tasks in the list.
```

### 4. Listing all tasks: `list`

Shows a list of all tasks in the task list.

Format: `list`

Example of usage: 

`list`

Expected outcome:
```
Here are the tasks in your list:
1.[T][✘] do assignment
2.[D][✘] have fun (by: June 1 2020)
3.[E][✘] attend conference (at: Jan 1 2020)
```

### 5. Marking a task as done: `done`

Marks the specified task as done.

The index refers to the index number shown in the displayed task list.

Format: `done INDEX`

Example of usage: 

`done 1`

Expected outcome:

```
Nice! I've marked this task as done:
  [T][✓] do assignment
```

### 6. Deleting a task: `delete`

Deletes the specified task from the task list.

The index refers to the index number shown in the displayed task list.

Format: `delete INDEX`

Example of usage: 

`delete 2`

Expected outcome:

```
Noted. I've removed this task:
  [D][✘] have fun (by: June 1 2020)
Now you have 2 tasks
```

### 7. Searching for a task: `find`

Finds tasks whose descriptions contain the given keyword.

Format: `find KEYWORD`

Example of usage: 

`find Assignment`

Expected outcome:

```
Here are the matching tasks in your list:
  [T][✓] do assignment
```

### 8. Undoing previous command: `sortAsc`
Sort the lists by ascending dates, dates of todo items are treated today.

Format: `sortAsc`

### 9. Redoing the previously undone command: `sortDes`
Sort the lists by ascending dates, dates of todo items are treated today.

Format: `sortDes`

### 12. Saving the data
The lists are automatically saved in a txt file and loaded everytime the programme starts.
