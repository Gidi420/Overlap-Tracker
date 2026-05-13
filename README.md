# Overlap Plan Improvement Tracker

A single-file project management dashboard for tracking improvements across a 5-chapter document. No build tools, no dependencies — just open `index.html`.

## Features

- **5-level hierarchy**: Project → Chapters → Sub-chapters → Tasks
- **Auto-calculated status**: Sub-chapter and chapter statuses roll up from task statuses
- **Inline editing**: Double-click any title to rename (Hebrew/RTL supported)
- **Task details**: Assignee, status, priority, due date, notes — expand any task row
- **Drag to reorder** tasks within a sub-chapter
- **Filters**: Search, status, priority, assignee, clickable stat pills
- **Activity log**: Last 20 changes with timestamps
- **Export/Import**: Full JSON backup and restore
- **Print/PDF**: Clean print stylesheet via ⎙ Print button
- **localStorage persistence**: Nothing lost on refresh

## Setup

### Option A — Open locally
```
Double-click index.html
```

### Option B — GitHub Pages
1. Create a new GitHub repository
2. Push `index.html` (and this README) to the `main` branch
3. Go to **Settings → Pages → Source → Deploy from branch → main / root**
4. Your dashboard will be live at `https://<your-username>.github.io/<repo-name>/`

## Usage

| Action | How |
|--------|-----|
| Rename anything | Double-click the title |
| Add chapter | Sidebar bottom button or "+ Add Chapter" |
| Add sub-chapter | "+Sub" button on chapter header |
| Add task | Press Enter in the "Add task…" input |
| Edit task fields | Click ⋯ on any task row to expand details |
| Reorder tasks | Drag the ⠿ handle |
| Filter | Use the pills, dropdowns, or search bar |
| Backup data | ↓ Export button |
| Restore data | ↑ Import button (drag a `.json` backup) |

## Data

All data is stored in `localStorage` under the key `overlap_tracker_v1`. Use Export/Import to move data between browsers or devices.
