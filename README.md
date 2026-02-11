# Todoist Time Scheduler Dashboard

A minimal, single-file dashboard for visualizing and organizing your Todoist tasks by energy level and priority — inspired by Kanban productivity methods for ADHD brains.

![Dashboard Preview](https://img.shields.io/badge/stack-HTML%20%2F%20CSS%20%2F%20JS-blue) ![No Dependencies](https://img.shields.io/badge/dependencies-none-green)

## Features

- **Energy-based task grouping** — tasks are categorized by labels like High Pressure, Draining, Energizing, Interesting, Boring, etc.
- **Daily Highlight hero card** — a full-width prominent card at the top for your `#dailyhighlight` task of the day
- **Live Todoist sync** — fetches your real tasks via the Todoist REST API with one click
- **Time estimation tracking** — see total estimated time per group and overall
- **Smart date display** — time ranges for scheduled tasks, color-coded due status (overdue, today, upcoming, future)
- **Filter chips** — quickly filter by label group
- **Priority indicators** — color-coded priority bars (p1–p4)
- **Meta-label tracking** — footnotes show how many tasks still need a label (`getmealabel`) or a date (`gimmeadate`)
- **Responsive design** — works on desktop and mobile
- **Zero dependencies** — pure HTML, CSS, and vanilla JavaScript in a single file

## How to Use

1. Open `index.html` in your browser
2. Click the **gear icon** (⚙) and paste your Todoist API token
   - Find it at: **Todoist Settings → Integrations → Developer → API token**
3. Click **Update** to fetch your live tasks
4. Your token is stored in your browser's `localStorage` — you only need to enter it once per browser

### Todoist Labels Setup

Create these labels in Todoist to organize your tasks by energy:

| Label | Purpose |
|-------|---------|
| `High Pressure` | Urgent & important tasks |
| `Deadline` | Tasks with hard deadlines |
| `Draining` | Energy-draining tasks |
| `energizing` | Energy-giving tasks |
| `interesting` | Interesting tasks |
| `Boring` | Low-energy tasks |
| `books` | Books to read |
| `movie` | Movies to watch |
| `dailyhighlight` | Your one key task for the day (shown as hero card) |

Meta-labels for task hygiene:

| Label | Purpose |
|-------|---------|
| `getmealabel` | Task needs a proper energy label |
| `gimmeadate` | Task needs a due date |

## Privacy & Security

- **No server, no backend** — everything runs client-side in your browser
- **Your API token never leaves your browser** — stored only in `localStorage`, never in the source code
- **The hardcoded task array** in the file is demo/fallback data only — replaced with your live data on first sync

## Credits & Inspiration

This dashboard is inspired by **Ruri Ohama**'s Kanban productivity method for ADHD brains, which focuses on organizing tasks by energy levels rather than rigid schedules.

Watch the original video: [Ruri Ohama — Kanban Method for ADHD](https://www.youtube.com/watch?v=WW8M9SbMTeE&t=0s)

## License

MIT
