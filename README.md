# CA Final FR Command Centre (PWA)

A small, installable Progressive Web App for the CA Final Financial Reporting plan ending 30 November 2026.

## Features
- Daily syllabus checklist and overall completion percentage
- Revision checklist, daily study-hour target and notes/error log
- Progress and notes saved in the browser's `localStorage`
- JSON backup export/import
- Service worker for offline loading after the first successful visit
- Android installation through Chrome

## Deploy free using GitHub Pages
You need a GitHub account. No build step or command line is required.

1. Download and extract `ca-fr-study-planner-pwa.zip`.
2. On GitHub, create a new **public repository** named `ca-fr-study-planner`.
3. Upload all files from this folder to the repository root (not the enclosing folder).
4. In the repository, open **Settings → Pages**.
5. Under **Build and deployment**, choose **Deploy from a branch**.
6. Select branch **main**, folder **/(root)**, then **Save**.
7. Wait for GitHub Pages to publish the site. The URL will look like:
   `https://YOUR-USERNAME.github.io/ca-fr-study-planner/`
8. Open that URL in Chrome on your Android phone. Wait for the page to load once online.
9. In Chrome, tap **⋮ → Install app** or **⋮ → Add to Home screen**.

GitHub Pages is HTTPS, which is required for service workers and normal PWA installation. Publishing menus can change slightly over time.

## Data and privacy
- Study progress and notes stay in the browser on that device, in localStorage. They are not automatically synced to another device.
- Export a JSON backup from the **Backup** tab. Store it somewhere safe.
- Use the import option on another device to restore a backup.
- Clearing Chrome site data may erase progress; export a backup first.
- Do not enter sensitive personal information in the notes.

## Important limitations
- This project creates the app files but does not publish them to the internet. You must complete the GitHub Pages steps above (or use another HTTPS static host).
- The timetable is a planning template. Adjust dates if you begin later or have already completed topics.
- Browser localStorage is suitable for a personal planner but is not a cloud backup.
