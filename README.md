# trueswing-frontend-archive

Read-only archive of the original TrueSwing web frontend.

This is the `frontend/` subtree of [oskarjolofsson/GSA1.0](https://github.com/oskarjolofsson/GSA1.0), extracted with `git subtree split` so the old app stays browsable without checking out an old SHA. It is not maintained, not deployed, and not accepting changes.

## What it was

A React 19 + Vite single-page app — the first user-facing TrueSwing client. Material UI and Emotion for components, Framer Motion for animation, React Router for navigation, Recharts for charts, and `@ffmpeg/ffmpeg` for in-browser video handling of swing uploads. Supabase and Firebase provided auth and storage. Tests ran on Vitest.

- Active: 2025-07-09 to 2026-06-27
- 453 commits touching the tree in the source repo

## Why it was archived

It was superseded by two purpose-built clients:

- `TrueSwing-expo-app/` — the React Native app that replaced it for players
- `trueswing_admin/` — the internal admin surface

By mid-2026 nothing depended on `frontend/` and no one had touched it in ten weeks, but it still surfaced in greps, in graphify output, and in documentation sweeps of the main repo. It was removed there in [GSA1.0#155](https://github.com/oskarjolofsson/GSA1.0/issues/155), and pushed here first so the code stays easy to read.

History was never at risk: every one of those 453 commits remains in `git log` in the source repo. This archive is for convenience, not safety.

## Running it

Possible but unsupported — the dependencies are pinned to their mid-2026 versions and the backend API it talked to has moved on.

```
npm install
npm run dev
```

It expects Supabase and Firebase credentials that are no longer provisioned.

---

Archived 2026-09-05.
