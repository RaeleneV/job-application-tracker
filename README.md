# 🗂️ Dossier — Job Application Tracker

A single-page tracker for managing a job search from first lead to final outcome — built while I job hunt during my final year of BSc Information Science (Informatics) at the University of Pretoria.

## Why

Job hunting generates a lot of scattered state: roles you're considering, ones you've applied to, interviews to prep for, offers, and rejections worth learning from. Dossier keeps all of it in one place instead of spread across notes apps, email folders, and memory.

## Features

- **Opportunities** — log a role's title, location, link, and notes as soon as you find it.
- **Applied** — mark an opportunity as applied (with a date), then track its outcome with independent status checks:
  - **Interview** — date, time, and any prep documents or images
  - **Accepted** — offer documents or images
  - **Rejected** — reasons or feedback, so patterns are easy to spot later
- **Documents** — a shared folder for the general things every application needs (CV, cover letter, ID, transcripts) rather than re-attaching them per job.
- Every job expands to show everything logged against it, in one consistent layout across every list.
- Light/dark mode follows your system preference.

## Tech stack

- Plain HTML, CSS, and vanilla JavaScript — no build step, no framework.
- Data storage: currently in-browser (IndexedDB), with a planned move to **Firebase (Firestore + Storage)** so the tracker can be shared live between me and a friend helping with the search.

## Status

🚧 In progress. Currently working end-to-end with local, per-browser storage. Next step is wiring in Firebase so two people can use it together with live sync.

## Running it locally

No build tools needed — just open `index.html` in a browser, or serve the folder with any static server:

```bash
npx serve .
```

## Roadmap

- [ ] Firebase Firestore for shared, real-time job data
- [ ] Firebase Storage for shared document/image uploads
- [ ] Basic auth (Google sign-in) restricted to specific collaborators
- [ ] Deploy via GitHub Pages or Firebase Hosting
