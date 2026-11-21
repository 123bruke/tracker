# Daymark — Task Manager

Daymark is a polished, browser-based task manager for planning work, organizing routines, and tracking progress. It runs as a single HTML file and keeps tasks on the user's device without requiring a server or account.

> A fast, private workspace for turning plans into completed tasks.

## Features

- Create, edit, complete, reopen, and delete tasks
- Schedule tasks for today, tomorrow, or an upcoming date
- Set task categories and priorities
- Add descriptions, progress percentages, and statuses
- Break larger tasks into individual subtasks
- Repeat completed tasks automatically every day
- Filter tasks by category or workspace view
- Search tasks by name or description
- View totals, completed work, today's tasks, and overdue work
- Track progress with a visual completion ring
- See an upcoming schedule in the side panel
- Export task data as JSON
- Import a compatible Daymark JSON backup
- Store data locally in the browser

## Screenshots

Screenshots can be added after opening the app and saving images of its main dashboard and task form.

```markdown
![Daymark dashboard](docs/images/dashboard.png)
![Create task dialog](docs/images/create-task.png)
```

## Getting Started

No build process or package installation is required.

### Open the app directly

1. Download or clone this repository.
2. Open `daymark_task_manager_fixed (1).html` in a modern browser.

### Run a local server

```bash
git clone https://github.com/123bruke/tracker.git
cd tracker
python3 -m http.server 8000
```

Then visit:

```text
http://localhost:8000/daymark_task_manager_fixed%20(1).html
```

## Using Daymark

1. Select **Add task** to open the task form.
2. Enter a task name and schedule date.
3. Optionally add a description, category, priority, time, progress, status, and subtasks.
4. Enable **Repeat every day** to create a fresh copy after completion.
5. Use the sidebar to browse All Tasks, Today, Tomorrow, Upcoming, or Completed tasks.
6. Filter the visible list by category or search by name and description.
7. Use the export control to download a JSON backup.
8. Use the import control to restore tasks from a compatible backup.

## Task Views

| View | Purpose |
| --- | --- |
| All tasks | Shows the full task workspace |
| Today | Shows tasks scheduled for the current day |
| Tomorrow | Shows tasks scheduled for the next day |
| Upcoming | Shows unfinished tasks scheduled after today |
| Completed | Shows tasks marked as completed |

## Task Categories

- General
- Normal
- Daily routine
- Quick wins
- Large projects

## Data Storage

Daymark tries the following browser storage options in this order:

1. `localStorage` for persistent storage on the current browser and device
2. `sessionStorage` for storage limited to the current tab
3. Browser window name storage as an additional fallback

Task data is stored only in the browser. Clearing browser data can remove saved tasks.

## Export and Import

Use **Export your data** to download tasks as a JSON file. The export includes the app name, a format version, export date, and task array.

Use **Import** to choose a compatible Daymark JSON backup. Existing tasks with matching IDs are updated; other imported tasks are added.

## Project Structure

```text
tracker/
└── daymark_task_manager_fixed (1).html  # Application UI, styles, and JavaScript
```

The application contains no build dependencies. HTML, CSS, and JavaScript are included directly in the single file.

## Browser Support

Daymark uses standard HTML, CSS, and JavaScript APIs. It should work in current desktop and mobile versions of major browsers.

## Privacy

Daymark does not send task information to a server. Task data remains in browser storage until it is exported or browser data is cleared.

## License

No license has been specified for this repository.
