# Daymark — Personal Tasks App

<!-- GitHub Repository -->
https://github.com/Dark0-0-1/DayMark.git



A simple personal to-do list built with React to practice component structure,
state management with hooks, and browser storage.

## Tech stack / libraries
- React 18 (functional components + hooks: `useState`, `useEffect`)
- Vite (build tool / dev server)
- Plain CSS (no UI framework)
- Browser `localStorage` for persistence (no backend/database)

## Features / modules implemented
1. **Add Task** — form with title (required), category (Work/Personal/Urgent/Study),
   and due date. Shows a validation message if the title is empty.
2. **Stats bar** — live counts for Remaining, Completed, Overdue, and Total tasks.
3. **Filters** — status tabs (All / Active / Completed) and category pills.
4. **Task list** — each task shows title, category chip, and due date.
   - Checkbox to mark complete (strikethrough style)
   - Edit button (inline rename)
   - Delete button
   - Drag-and-drop to manually reorder tasks
   - Overdue tasks are highlighted automatically (due date in the past and not completed)
5. **Theme toggle** — light/dark mode, remembered across visits.
6. **Persistence** — all tasks and the theme choice are saved to `localStorage`,
   so they survive a page refresh.

## Setup instructions
1. Make sure [Node.js](https://nodejs.org) (v18+) is installed.
2. Unzip the project folder and open a terminal inside it.
3. Install dependencies:
   ```
   npm install
   ```
4. Start the development server:
   ```
   npm run dev
   ```
5. Open the printed local URL (usually `http://localhost:5173`) in your browser.

To create a production build:
```
npm run build
```
The output will be in the `dist/` folder.

## Project structure
```
daymark/
├── index.html
├── package.json
├── vite.config.js
├── README.md
└── src/
    ├── main.jsx
    ├── App.jsx
    ├── App.css
    ├── index.css
    └── components/
        ├── TaskForm.jsx
        ├── StatsBar.jsx
        ├── FilterBar.jsx
        ├── TaskList.jsx
        └── TaskItem.jsx
```
