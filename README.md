# Notes Offline Browser

A lightweight, offline-first note-taking experiment that runs entirely in the browser.

Open `index.html`, write your notes, organize them with categories and colors, and keep everything in a portable single-page workflow without installing anything.

The main purpose of this app is to test the idea of storing note data directly in the URL, instead of using a server or browser storage.

## Features

- Add, edit, delete, and reorder notes
- Mark important notes
- Organize notes with categories and custom colors
- Search, filter, and sort your notes
- Switch between Turkish and English
- Export and import notes as JSON
- Works locally in the browser without a backend

## Usage

Download or clone the repository, then open `index.html` in your browser.

No build step, package manager, server, or internet connection is required.

## Data Storage

The app intentionally stores note data in the page URL, inside the `?notes=...` parameter. This makes the current note state portable and shareable as a link, while keeping the app as a single static HTML file.

This is an experimental design choice. It does not use a backend database or `localStorage` for note data, and it does not send your notes to a server.

URLs have practical length limits that vary by browser, bookmark manager, chat app, and operating system. When the URL becomes too long, saving new changes may fail. Use JSON export/import as a backup or transfer option for larger note sets.

## Recommended Workflow

1. Open `index.html`.
2. Add notes with a title, category, color, and content.
3. Use search, filters, and sorting to browse your notes.
4. Export your notes as JSON when you want a backup.

## Project Structure

```text
.
├── index.html
└── README.md
```

## License

No license has been specified yet.
