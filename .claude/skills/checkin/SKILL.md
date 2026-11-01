---
name: checkin
description: Evening review. Ask how the day went, append an entry to data/log.md, and once a week distill patterns into data/learnings.md.
---

# Check-in

1. Read today's `plans/YYYY-MM-DD.md` (if there is one) and `data/log.md`.
2. Ask in **one short message**, keeping it phone-friendly:
   - "What got done today? (✅ the blocks, or just tell me)"
   - "Energy 1–5?"
   - "Anything to note, or any errand or chore to schedule this week?"
3. Append to `data/log.md` in the format of `data/log.example.md`:
   ```
   ## YYYY-MM-DD (Day)
   - Done: …
   - Skipped: …
   - Energy: n/5
   - Notes: …
   ```
4. If the user mentions a lasting preference, update `data/profile.md`. If they mention an errand, note it for the next `/plan-day`.
5. **Weekly (Saturday, or when there are 7+ new entries since the last update):** re-read the week's log, then rewrite `data/learnings.md` with 3–6 short, concrete patterns, in the format of `data/learnings.example.md`.
6. Reply with one warm line, plus one tiny win you noticed in the day.
