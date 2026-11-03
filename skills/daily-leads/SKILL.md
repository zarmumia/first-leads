---
name: daily-leads
description: The daily routine of First Leads. Use when the user says "today's leads", "find posts for me", "daily routine", "what should I comment on today", "find Upwork jobs", "LinkedIn leads", or "do my comments". Scans the user's chosen channels for fresh posts and jobs that fit, scores them, drafts replies in the user's voice for the user to send, and logs what was sent.
---

# Daily routine: new conversations

Read before starting:
- `${CLAUDE_PLUGIN_ROOT}/skills/first-leads/references/platform-rules.md`
- `${CLAUDE_PLUGIN_ROOT}/skills/first-leads/references/method.md`
- `first-leads/profile.md`, `first-leads/channels.md`, and today's counts in `first-leads/progress.md`
- `${CLAUDE_PLUGIN_ROOT}/skills/first-leads/references/goals.md`: adapt search signals, scoring and the open door of each draft to the goal in the profile

If follow-ups are due today (rows in `leads-log.csv` with `next_step_date` today or earlier), suggest doing those first with the follow-ups skill: an existing conversation is worth more than a new one.

## Steps

1. **Ask which channels today** (default: all in `channels.md`), and remind the user of the time budget from the profile.
2. **Read** each chosen place with the user's logged-in browser, only now that the user asked, one page at a time, at a human pace, within the reading limits in the platform rules (about 10 pages per channel per session). Never run this routine unattended or on a schedule. The user can also open any page themselves and say "check this page". Use the channel guide:
   - Facebook groups → `references/facebook.md`
   - LinkedIn → `references/linkedin.md`
   - Upwork → `references/upwork.md`
   - Forums → read the thread, follow the community's rules in `channels.md`
3. **Score** every candidate as in the method. Show only scores 4–5, best first, at most the daily limit for each channel.
4. **For each pick, show:** where it is (group/site + link), who posted and when, a one-line summary of what they need, why it fits, and the draft.
5. **Let the user edit.** If they change the wording, keep it. If the change shows a voice pattern (a word they always remove, a tone they prefer), offer to add it to the "Voice" section of the profile.
6. **The user sends.** Offer to open the post. If the user asks you to place the draft in the box, type it with Shift+Enter for line breaks, never press Enter, never click Send, and tell them it is waiting for them.
7. **Log** each item the user confirms as sent in `leads-log.csv` with status `sent` and a `next_step_date` (usually 2–3 days later, to check for replies). Items not sent are not logged.
8. **Close the session:** update today's counts in `progress.md`, say what was done in one line, and when to come back.

## Stop conditions

- Daily limit reached for a channel.
- Nothing scores 4 or above: say so. Do not lower the bar to fill the list; suggest checking again later or adding a place.
- The user asks to send automatically or in bulk: refuse per the platform rules and offer the allowed way.
