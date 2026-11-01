# Moti schedule
Read by `/start`. Edit the times here, then run `/start` again.
Times are local (Asia/Jerusalem). Jobs are session-only and expire after 7 days, so re-run `/start` after a restart or each week.

| Job | Time | Days | Prompt |
|-----|------|------|--------|
| morning-plan | 08:37 | every day | Moti morning run: follow `.claude/skills/plan-day/SKILL.md` for today. Then send ONE PushNotification under 200 chars with the day's 3–4 key blocks, e.g. "🗓️ Today: job search 9:00 · Nebius 13:30 · 📅 dentist 17:00. Open Moti to adjust." Ask the Propose-mode questions in the session reply, not in the notification. |
| evening-checkin | 21:43 | every day | Moti evening check-in: follow `.claude/skills/checkin/SKILL.md` steps 1–2. Send ONE PushNotification under 200 chars, e.g. "🌙 Check-in time! How did today go? Reply in Moti: done, energy 1–5, notes." Wait for the user's answer before writing the log. |
