# Moti 🗓️

A personal day-planning agent for the job-hunting period. It gets to know you, proposes a daily plan around your Google Calendar, and learns from how your days actually go.

Built step by step as a hands-on way to learn AI agent engineering.

## How it works
- **Know the user:** `/onboard` interviews you and writes `data/profile.md`.
- **Plan:** `/plan-day` reads the profile, learnings, log and Google Calendar, then writes `plans/YYYY-MM-DD.md`.
- **Learn:** `/checkin` logs the day and distills patterns into `data/learnings.md` weekly.
- **Two modes:** *Propose* for the first 7 logged days (explains its reasoning and asks for feedback), then *Smart* (plans confidently from learnings).

Personal data (`data/`, `plans/`) is git-ignored and stays local.

## Roadmap
1. ✅ Claude Code native: `CLAUDE.md` + skills
2. ⬜ Python + Claude Agent SDK rebuild
3. ⬜ Write approved plans to Google Calendar

## Use
Open the folder in [Claude Code](https://claude.com/claude-code), run `/onboard`, then `/plan-day`.
