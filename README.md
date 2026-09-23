# LVAEP Session Log

A lightweight replacement for LVAEP's paper-based Student Monthly Attendance & Achievement Form. Tutors record one session at a time, and staff receive an immediate monthly summary by student.

## Live demo

[https://lvaep-session-log.hi-ryanpang.chatgpt.site](https://lvaep-session-log.hi-ryanpang.chatgpt.site)

## Features

- Record a tutoring session with student, date, duration, and an optional note
- Filter records by reporting month
- See monthly totals for hours, sessions, and active students
- Review totals by student
- Delete incorrect entries with confirmation
- Persist records in the browser with `localStorage`
- Responsive, keyboard-friendly interface
- Seeded sample records make the workflow immediately demonstrable

## Run locally

No build step or dependencies are required.

```bash
python3 -m http.server 4173 --directory dist
```

Then open `http://localhost:4173`.

## Product decisions

This prototype focuses on the highest-frequency workflow: recording sessions and preparing monthly attendance totals. It deliberately avoids authentication, a shared database, PDF export, and the full achievement-goal checklist so the core interaction remains complete and reliable within the take-home timebox.

For a production version, the next step would be a shared database with tutor accounts, student assignments, achievement tracking, and CSV/PDF exports for staff.

## Tech stack

- Semantic HTML
- Modern CSS
- Vanilla JavaScript
- Browser `localStorage`

## Data note

All names and records in the demo are fictional. Data is stored only in the current browser.
