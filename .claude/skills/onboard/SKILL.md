---
name: onboard
description: Interview the user to learn their routine, duties, goals and interests, and write data/profile.md. Use first, or to update the profile.
---

# Onboard

Goal: know the user well enough to plan their days.

1. If `data/profile.md` has content, show a short summary and ask what changed. Edit only those parts.
2. Otherwise, interview in **4 short rounds** of 2–4 questions each. Wait for answers between rounds.
   - **Rhythm:** wake and sleep times, best focus hours, fixed commitments (days and times).
   - **Job search and growth:** CV goal (e.g. how many per day or week), what to study, side projects (e.g. the moti Claude project).
   - **Home and life:** chores and how often (cleaning, groceries, cooking), family and friends visits.
   - **Joy and body:** hobbies, games, walks or sport, what recharges you, what drains you.
3. Suggest sensible defaults when an answer is vague ("1×/week groceries, Sunday?").
4. Write `data/profile.md` in exactly this structure:

```markdown
# Profile
_Updated: YYYY-MM-DD_

## Rhythm
- Wake: … | Sleep: … | Best focus: …

## Fixed
- <what> — <when>

## Daily goals
- <what> — <amount/duration>

## Recurring
- <what> — <frequency> (<preferred day/time>)

## Leisure & body
- <what> — <notes>

## Constraints & notes
- …
```

5. Finish with a 3-line summary and: "Ready! Run `/plan-day` when you want your first plan."
