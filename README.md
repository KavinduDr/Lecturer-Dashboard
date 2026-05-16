# Software Project Admin

An admin dashboard web app for managing quizzes and essay assessments, built with Next.js (14), React (18) and Tailwind CSS.

This repository contains a server-rendered and client-interactive Next.js application used to create and manage quizzes, view student results, and handle essay-type answers.

## Key Features

- Admin dashboard and routes for creating and editing quizzes and essays.
- Student result views (per-quiz and per-student) and essay result pages.
- Authentication-related pages: `signup`, `forgot-password`, `reset-password`, and `activate`.
- Reusable UI primitives and Radix/NextUI-based components under `app/components/ui`.
- Context providers for application state: `AdminContext`, `QuizContext`, `EssayContext`.

## Project structure (high level)

- `app/` — Next.js app routes and UI components.
- `app/components/` — shared components and small UI modules.
- `app/context/` — React context providers for app-wide state.
- `app/dashboard`, `app/viewquiz`, `app/viewResult`, `app/viewEssayResult` — main feature areas for administration and reporting.
- `public/` — static assets and images.

## Requirements

- Node.js 18 or later
- npm (or yarn / pnpm)

## Install & Run

Install dependencies and run the development server:

```bash
npm install
npm run dev
```

Open http://localhost:3000 in your browser.

Available npm scripts (from `package.json`):

- `dev` — run development server (next dev)
- `build` — build production bundle (next build)
- `start` — start production server (next start)
- `lint` — run linter (next lint)

## Build & Production

Build the app for production and run it locally:

```bash
npm run build
npm start
```

## Notes for contributors

- UI components live in `app/components/ui` — follow existing patterns when adding new primitives.
- Context providers are in `app/context` — add or extend providers when new global state is required.
- Keep styles consistent with Tailwind and existing design tokens in `tailwind.config.ts`.

If you'd like, I can also add a CONTRIBUTING.md with PR guidelines and a small developer setup checklist.

---

Original scaffolded README updated to reflect this project's structure and run instructions.
