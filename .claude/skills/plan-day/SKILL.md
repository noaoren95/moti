---
name: plan-day
description: Build today's (or a given day's) plan from the profile, learnings, log and Google Calendar, and save it to plans/YYYY-MM-DD.md.
---

# Plan day

1. **Gather context**
   - Read `data/profile.md` (if it's empty → ask the user to run `/onboard`), `data/learnings.md` and `data/log.md`.
   - Read the Google Calendar events for the target day, in the user's timezone. These are **fixed**. Add a 15-minute buffer around each and travel time if the event is outside the home.
   - Look at this week's existing `plans/` files and log entries (the week runs Sun–Sat) to see which weekly quotas are already done: cleaning, groceries, cooking, family.
2. **Pick the mode:** fewer than 7 log entries → Propose. Otherwise → Smart (see CLAUDE.md).
3. **Build the day** between wake and sleep:
   - Weekday (Sun–Thu): put job search in the first focus window, deep study in the second, and a short job-search check in the afternoon.
   - Weekend (Fri–Sat): no job search. Plan chores, family, people and leisure.
   - Spread the weekly quotas sensibly. Don't stack them all on the last day.
   - Every day: meals, breaks, movement, and games ≤ 60 min. Leave ~1h of unplanned buffer, but no long empty gaps.
   - Suggest one people-related idea when the day or week has none (call someone, a meetup, a class).
4. **Output** in the terminal, then save to `plans/YYYY-MM-DD.md`:

```markdown
# Plan: <Weekday> YYYY-MM-DD  (<mode> mode)
| Time | Block | Note |
|------|-------|------|
| 08:30 | Wake up, breakfast | |
...
**Weekly quotas:** cleaning ✅/⬜ · groceries ⬜ · cooking ⬜ · family ⬜
**Why this plan:** 2–3 bullets (Propose mode) or "changes since last time" (Smart mode)
```

5. In Propose mode, end with 1–2 questions, e.g. "Does the study length feel right?" Apply the answers to the plan and, if they're lasting preferences, to `data/profile.md`.
