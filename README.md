# World Cup 2026 — Bracket & Win Probability

A single, self-contained, **zero-dependency** web app: pick any of the 48 teams at the 2026 FIFA World Cup to see its possible knockout opponents round-by-round, what-if paths, and model-based win probabilities (in-browser Monte-Carlo).

- **No framework, no build step** — just `index.html`. Plain HTML/CSS/JS.
- Mobile-first, accessible (keyboard nav, ARIA combobox, focus states, reduced-motion).
- Title-race leaderboard, per-country probability dashboard, swipeable bracket, 1-hour result cache.

## Run locally

Open `index.html` in any browser, or serve it:

```bash
npx serve .
```

## Deploy

Static site — Vercel serves `index.html` directly, no build configuration needed.

## Editing the data

Group standings and team strength ratings live in the `DATA` section near the top of the `<script>` in `index.html`. Update `GROUPS`, `LOCK`, and `RATING` as results come in.

> ⚠️ Win probabilities are a heuristic Monte-Carlo model (team strength ratings + current standings) — an estimate, not official odds.
