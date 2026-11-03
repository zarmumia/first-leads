---
name: follow-ups
description: Follow-up step of First Leads. Use when the user says "who should I follow up with", "follow-ups for today", "someone replied to me", "draft a WhatsApp follow-up", "a lead went quiet", or "update my lead log". Finds leads due for a follow-up, helps the user answer replies, drafts one personal follow-up message per person (WhatsApp, DM, LinkedIn or Upwork), and keeps the lead log current.
---

# Follow-ups

A conversation that already started is worth more than a new comment. This skill makes sure no reply is missed and no warm lead goes quiet because nobody came back.

Read `${CLAUDE_PLUGIN_ROOT}/skills/first-leads/references/platform-rules.md` and `first-leads/profile.md` first.

## Steps

1. **Ask what happened since last time.** "Did anyone reply, message you, or call?" Update `leads-log.csv`: `replied`, `conversation`, `meeting`, `client`, `no_reply`, `not_a_fit`.
   If the user asks, check the original threads in the browser for replies (read only).
2. **List who is due today:** rows with `next_step_date` today or earlier and status `sent`, `replied` or `conversation`. Respect the daily follow-up limit.
3. **For each person, draft one message** for the right channel:
   - **Reply in a thread** → answer their reply in the same thread.
   - **WhatsApp / DM** → only if this person contacted the user there or gave their number. Short, personal, referring to what they said.
   - **LinkedIn** → continue the existing exchange; no pitch in the first message after connecting.
   - **Upwork** → inside Upwork only.
4. **What a good follow-up looks like:**
   - Refers to something specific they said.
   - Adds something new (a tip, a template, an answer to their objection), not "just checking in".
   - Has one clear, easy next step (a short call, a yes/no question, a time).
   - 2–5 lines.
5. **Limits:** at most 2 follow-ups per person without a reply, at least 3 days apart. After that, mark `no_reply` and let it go. If someone says no, mark `not_a_fit` and never contact them again.
6. **The user sends** each message from their own phone or account. If they ask you to place a draft in a box in the browser, use Shift+Enter for line breaks and never press Enter or click Send.
7. **Log** what was sent and set the next `next_step_date`. Update `progress.md`.

## When a lead becomes a conversation

Help the user prepare: a short summary of what the person asked and said (read from the thread through the link; do not save their name or details in the files), two or three questions to understand their situation, and one simple proposal for a next step. Remind the user: the goal of the first call is to understand, not to sell everything.
