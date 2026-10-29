# Education Radar

A weekly education news briefing, in English. Every Monday it scans global education news from the past 7 days and gives an analysis of the three most important items, plus a list of other items on the radar.

## How it works

- `prompt.md` is the full instruction set for the weekly run (a Claude scheduled task, `0 8 * * 1`, local time).
- Each run saves its briefing as `docs/reports/<year>-W<week>.md`, updates `docs/reports.json`, then commits and pushes.
- `docs/index.html` is the website (GitHub Pages, served from `docs/`): it shows the latest briefing and an archive.

Site: https://gsleraar-hue.github.io/education-radar/

## Briefing structure

1. Week in one glance
2. Top 3 with analysis: what happened, why it matters, context, what to watch
3. Insight for the LessonUp team
4. Also on the radar (8-12 one-liners with sources)

## Setup

Create a Claude scheduled task with the contents of `prompt.md` and cron `0 8 * * 1`. The app must be open for the task to run.
