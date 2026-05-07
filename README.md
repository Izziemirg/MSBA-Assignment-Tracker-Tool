## Task Matrix | MSBA Planner

A lightweight, single-file task manager built for busy MSBA students. No backend, no accounts, no setup, just open and go.


## Features

Add tasks with a name, due date, category, and priority in seconds
Automatic urgency sorting, overdue and high-priority tasks float to the top
Color-coded deadline labels, overdue in red, due soon in amber, everything else calm
Focus Mode, collapses your list to just the 3 most urgent tasks to reduce overwhelm
Category filters, view only Homework, Exams, Group Meetings, or Reading at a time
Progress bar, see your daily completion percentage at a glance
Per-user isolation, each user logs in with their name and a 4-digit PIN; tasks are stored privately and separately on the device
Persistent storage, tasks survive page refreshes via localStorage
Dark mode, automatically follows your OS system preference
Fully responsive, works on mobile and desktop


## How user isolation works

There is no server or database. All data lives in your browser's localStorage. When you log in, your name and PIN are combined into a unique storage key — so your tasks are never mixed with another user's, even on a shared device. Importantly, PINs are not recoverable — if you forget your PIN, your tasks cannot be retrieved (you would simply start fresh with a new PIN).

Deploying to GitHub Pages

Fork or clone this repo
Make sure the file is named index.html (rename task-matrix.html if needed)
Go to your repo's Settings → Pages
Under Source, select main branch and / (root) folder
Click Save — your site will be live at:

https://<your-username>.github.io/<your-repo-name>
It may take 1–2 minutes for GitHub Pages to deploy on the first push.

Local development
No build step or dependencies needed. Just open the file directly in your browser:
bashopen index.html
# or on Windows:
start index.html

External dependencies (CDN)
The tool loads two resources at runtime — no npm install required:
ResourcePurposeGoogle Fonts (Syne + Space Mono)TypographyTabler Icons via cdnjsUI icons
Both load from public CDNs. The tool will still function (with fallback fonts and no icons) in offline mode.

Project structure
index.html      # The entire app — HTML, CSS, and JS in one file
README.md       # This file

Built for
BACS / UX Design coursework — digital tool design assignment.
Designed to address cognitive overload, task capture failure, and deadline blindness in MSBA students.

License
MIT — free to use, fork, and adapt.
