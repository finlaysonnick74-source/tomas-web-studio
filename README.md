# Tomas Web Studio

Live site: https://finlaysonnick74-source.github.io/tomas-web-studio/

## Updating the daily tracker

All 21 days live in **progress.json**. Each day looks like this:

```json
{ "day": 1, "date": "2026-10-17", "plan": "Write the brief for my own site",
  "status": "done", "built": "...", "learned": "...", "proud": "...",
  "commit": "https://github.com/finlaysonnick74-source/tomas-web-studio/commit/...", "dad_note": "" }
```

Each day:
1. Open `progress.json` and find today.
2. Set `status` to `"progress"` when you start, `"done"` when you finish (others stay `"upcoming"`).
3. Fill in `built`, `learned`, `proud`. Dad can add `dad_note` (optional).
4. Commit and push:
   ```bash
   git add progress.json && git commit -m "Day 1 done" && git push
   ```
5. Copy the commit link into `commit` (next push is fine).

GitHub Pages rebuilds in about a minute. The tracker page reads `progress.json` and updates the calendar, progress bar and streak by itself.

Tip: keep the JSON valid (commas between fields, double quotes). If the tracker goes blank, check for a missing comma.
