# Basecamp

A single-file calorie & body-weight tracker with a mountain-climb metaphor
(trailhead → summit). No build step — everything lives in `index.html`
(HTML + CSS + vanilla JS). Data syncs to your Dropbox via PKCE OAuth, with
`/data.json` as the source of truth, so entries can also be added from chat.

## Features

- **Calories in / out** — log food and activity, with BMR → TDEE → daily
  target (Mifflin-St Jeor) and a live remaining budget.
- **Macro tracking** — optional protein / carbs / fat per food entry, with
  per-day macro bars and targets (protein g/kg, fat % of calories, carbs as
  the remainder). Calorie-only entries still work; kcal auto-fills from macros
  when left blank.
- **Weight trend** — line chart with a 7-point moving average, goal line, and
  a projected goal date from the current trend (linear regression).
- **Weekly summary & streaks** — per-week average intake vs target, estimated
  weight change (7700 kcal ≈ 1 kg), and an on-target day streak.
- **Water tracking** — daily hydration against a goal, with quick +250/+500 ml.
- **Quick-add favorites** — one-tap re-logging of your most frequent foods.
- **Edit / delete** — fix or remove any food, activity, or weigh-in; log
  weight for past dates.
- **Dark mode** — theme toggle that follows the system preference by default.
- **Settings** — edit your profile (height, age, goal, activity, pace) and
  macro/water targets in-app.

## Running

Open `index.html` in a browser, or host it statically. Connect Dropbox to sync
across devices; otherwise data is cached in the browser only.
