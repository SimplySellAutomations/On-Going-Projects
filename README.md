# Project Tracker

A lightweight, single-file project tracker you can host on GitHub Pages and share with your team. No backend, no login — everything saves in the browser.

## Features

- **Table View** — sortable columns with progress bars, start dates, last update, and due dates
- **Status Board** — visual board grouped by status (like a Kanban but simpler)
- **Collapsible sub-projects** — parent projects like Salesforce can be expanded/collapsed
- **Status options** — Not Started, Started, In Progress, Under Review, Evaluating, On Hold, Completed
- **Date tracking** — Start/Assignment date, Last Update, and Due Date per project
- **Filter by status** — quickly focus on what matters
- **Add / Edit / Delete** — full CRUD via a modal form
- **Export CSV** — download your data for Excel or Google Sheets
- **Persists in browser** — data saves to localStorage automatically

## How to use

### Option 1: GitHub Pages (recommended, shareable link)

1. Create a new GitHub repository (e.g. `project-tracker`)
2. Upload `index.html` to the root of the repo
3. Go to **Settings → Pages → Source → Deploy from branch → main / root**
4. GitHub will give you a URL like `https://yourusername.github.io/project-tracker/`
5. Share that link with your team

### Option 2: Open locally

Just double-click `index.html` — it opens in any browser, no server needed.

## Customizing

All data and logic is in a single `index.html` file. To pre-load your own projects, edit the `defaultProjects` array near the top of the `<script>` tag.

## Notes

- Data is stored in `localStorage` — it persists per browser, not across devices
- To share updated data with teammates, use **Export CSV** and re-import manually, or consider hosting on GitHub Pages where each person manages their own view
- To reset to defaults, open browser DevTools → Application → Local Storage → delete the `project_tracker_v3` key

## License

MIT — free to use and modify.
