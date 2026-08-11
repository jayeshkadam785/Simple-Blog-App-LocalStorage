# Task 3: Simple Blog App with Local Storage

**Internship:** Software Development | SaiKet Systems
**Stack:** HTML, CSS, JavaScript (Browser `localStorage`)

## Objective
Develop a blog application that allows users to create, read, and delete posts, with data persisted locally using browser `localStorage`.

## Features
- Clean, card-based UI for writing and viewing posts
- **Create:** Add a post with title + content, saved instantly to `localStorage`
- **Read:** All saved posts render automatically on page load, newest first
- **Delete:** One-click delete per post, updates storage immediately
- Data persists across browser refreshes/sessions (until manually cleared)
- XSS-safe rendering (user input is escaped before display)
- Empty-state message when no posts exist
- Fully responsive, no external dependencies

## How to Run
1. Open `task3_blog_app.html` directly in any modern browser (Chrome, Edge, Firefox)
2. No server or build step required — pure client-side app

## How It Works
- Posts are stored as a JSON array under the `simpleBlogPosts` key in `localStorage`
- Each post has: `id` (timestamp), `title`, `content`, `date`
- `renderPosts()` re-reads storage and re-renders the list on every change

## Requirements
- Any modern web browser
- No installation, server, or internet connection needed
