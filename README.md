# Daymark — Task Manager

Daymark is a clean, responsive task manager that runs entirely in the browser. Create, schedule, categorize, and track tasks with priorities, progress levels, subtasks, recurring daily tasks, and productivity summaries.

## Features

- Create, edit, complete, reopen, and delete tasks
- Search tasks and filter by category
- Schedule tasks for today, tomorrow, or upcoming dates
- Assign priorities and track completion progress
- Break tasks into smaller subtasks
- Repeat tasks automatically each day when completed
- View completion, overdue, today, and upcoming task summaries
- Store tasks locally in the browser
- Export tasks as JSON
- Import tasks from a JSON export
- Responsive layout for desktop and mobile

## Getting Started

No build tools or dependencies are required.

1. Clone the repository:
   ```bash
   git clone https://github.com/123bruke/tracker.git
   ```
2. Open `daymark_task_manager_fixed (1).html` in a web browser.

Alternatively, serve the project with a local static server:

```bash
python3 -m http.server 8000
```

Then visit `http://localhost:8000/daymark_task_manager_fixed%20(1).html`.

## Usage

1. Select **Add task** to open the task form.
2. Enter a task name and schedule date.
3. Optionally add a description, category, priority, time, progress, status, and subtasks.
4. Enable **Repeat every day** if the task should continue automatically after completion.
5. Use the sidebar and category filters to find tasks.
6. Use the export button to download a JSON backup.
7. Use the import control to restore tasks from a compatible JSON file.

## Data Storage

Daymark tries to save tasks in this order:

1. Browser `localStorage` for persistent storage on the device
2. `sessionStorage` for storage limited to the current tab
3. Window name storage as a fallback

Task data is not sent to a server. Clearing browser data may permanently remove locally stored tasks, so export important task lists when needed.

## Project Structure

```text
tracker/
└── daymark_task_manager_fixed (1).html  # Complete application UI and logic
```

## Browser Support

The app uses standard HTML, CSS, and JavaScript APIs and should work in modern desktop and mobile browsers.

## License

No license has been specified for this repository.
