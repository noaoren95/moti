---
name: start
description: Start (or restart) Moti's scheduled jobs from schedule.md. Run after opening a session, after editing schedule.md, or when the jobs expire after 7 days.
---

# Start

1. Read `schedule.md`.
2. Run CronList. Delete (CronDelete) every existing job whose prompt starts with "Moti", so nothing is duplicated.
3. For each row, create a recurring job with CronCreate:
   - cron = `<minute> <hour> * * <days>` (every day = `*`, Sun–Thu = `0-4`)
   - prompt = the row's Prompt text
4. **Correct for jitter.** The scheduler may add a fixed delay of up to 30 minutes. If a job's reported next run is more than 5 minutes after the target Time, delete it and recreate it earlier by that delay. Do this once per job.
5. Report a short table (job · target time · actual next run) and remind the user:
   - keep this session open, with Remote Control connected for the phone
   - the jobs expire after 7 days (give the date), so run `/start` again then
