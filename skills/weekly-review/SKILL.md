---
name: weekly-review
description: Weekly learning step of First Leads. Use when the user says "weekly review", "what's working", "which groups bring leads", "my lead numbers", "should I change my approach", or when the coach sees a week has passed since the last review. Reads the lead log, shows which places and openings bring real conversations, and recommends what to keep, change or drop next week.
---

# Weekly review

Turn the lead log into decisions. Read `first-leads/leads-log.csv`, `first-leads/profile.md`, `first-leads/channels.md` and `first-leads/progress.md`.

## Steps

1. **Check there is enough data.** Fewer than 10 sent items: say it is too early to judge, and focus the review on consistency (did the user show up daily?).
2. **Count, for the period and in total:**
   - Sent per channel and per place.
   - Replies, conversations, meetings, clients per channel and per place.
   - The main number: **conversations per 10 sent**, per place.
   - The success number for each goal in the profile, separately (see `${CLAUDE_PLUGIN_ROOT}/skills/first-leads/references/goals.md`), using the `goal=` tag in the log's notes.
   - Follow-ups due that were missed.
3. **Show it simply:** a short table per place, then three to five plain-language findings, for example "Group X: 8 comments, 3 conversations — your best place. Group Y: 7 comments, nothing — drop it or try a different kind of post."
4. **Look at the wording:** which drafts got replies, and what they have in common (a concrete offer? a question? shorter?). Which edits the user keeps making.
5. **Check the rules are fresh.** List places in `channels.md` whose rules were read more than 30 days ago, and re-read them with the user. Once a month, offer to open each platform's official rules page together and note anything that changed (see "Rules change" in the platform rules).
6. **Check the spread.** If more than about 80% of conversations come from one channel, say so: it works, but it is a single point of failure. Suggest keeping a second channel alive, even at low volume.
7. **Recommend for next week** (at most three changes):
   - Places to keep, add, or drop (drop after two weeks with no conversations).
   - Search signals to sharpen in the profile.
   - A voice or structure change based on what got replies.
8. **Update with the user's approval:** `channels.md`, the "Search signals" and "Voice" sections of `profile.md`, and a dated summary in `progress.md`.

## Be honest

If the numbers are weak, say so plainly and suggest one concrete change. Do not inflate small results. If a place's rules changed or the user got a warning from a platform, stop using that place and review the platform rules together.
