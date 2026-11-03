---
name: onboarding-interview
description: First stage of First Leads. Use when the user says "set up my profile", "start the interview", "get to know my business", "update my target audience", or when the first-leads coach finds no profile yet. Interviews the user about their business, ideal client, the words clients use, where they hang out, and the user's own voice, then writes the profile every other step relies on.
---

# Getting to know you (onboarding interview)

Interview the user and write `first-leads/profile.md`. This profile is the specification for everything else: what to search for, how to score posts, and how drafts should sound.

Read `${CLAUDE_PLUGIN_ROOT}/skills/first-leads/references/method.md` first.

## How to run the interview

- Tell the user: "About 20 minutes. Answer in your own words; short answers are fine. If you don't know an answer, say so and we'll work it out together."
- Ask one section at a time, two or three questions per message, never the whole list at once.
- When an answer is vague ("small businesses", "anyone who needs marketing"), help the user sharpen it with a follow-up question or an example. Do not accept a vague answer for the ideal client or the pain language: these drive the search.
- Many new business owners cannot describe their audience yet. That is normal. Help them think: ask about their best client so far, or the last three people who asked them for help.
- Never invent answers. If something stays unknown, mark it `unknown - to learn` in the profile.

## The sections

**0. What are you looking for?** (ask first; it shapes every other question)
- Do you offer a service, or are you building a product?
- What do you need most right now: **clients**, **case-study / pilot partners**, **collaborations / partnerships**, or **early users and feedback**? More than one is fine; which comes first?
Read `${CLAUDE_PLUGIN_ROOT}/skills/first-leads/references/goals.md` and adapt the wording of the next sections to the goal (for example "ideal client" becomes "ideal pilot partner" or "ideal partner").

**1. The business**
- What do you sell, in one sentence?
- What does a typical deal cost?
- How many new clients a month do you want, and how many can you actually take?

**2. The right client**
- Who was your best client so far, and why?
- Who decides, and who pays?
- What happened to the client just before they looked for someone like you?

**3. The pain, in their words**
- How does a client describe the problem in their own words (not yours)? Ask for real sentences they have said or written.
- What have they usually tried before reaching you?
- What objection do you hear most?

**4. Where they are**
- Which Facebook groups, LinkedIn circles, forums or communities do your clients use?
- Are you on LinkedIn? On Upwork? Which do you already use?
- "I don't know" is a fine answer; the next stage finds out.

**5. Your voice**
- Paste 2–3 messages, posts or comments you wrote and liked.
- What would you never write? (words, tone, emojis, pushiness)

**6. Time and goal**
- How many minutes a day can you give this? (15–20 is enough.)
- What counts as success for you right now: a reply, a conversation, a meeting?

**7. The commitment**
Say: "The system finds, scores and drafts. You read, edit and send every message yourself. That keeps your accounts safe and keeps the conversation in your real voice. Does that work for you?"
If the user wants fully automatic sending, explain why it is not offered and stop the setup; this coach is not the right fit.

## Write the profile

Create the `first-leads` folder if needed and write `profile.md`:

```markdown
# Profile — <business name>
Updated: <date>

## Goal
<service|product> | Looking for: <clients / pilot partners / partnerships / early users>, first: <one>

## Offer
<one sentence> | Typical deal: <amount> | Capacity: <clients/month>

## Ideal client
<who, decision maker, payer, trigger moment>

## Pain language (their words)
- "<real phrase>"
- ...

## What they tried before / common objections
...

## Where they are (known so far)
...

## Voice
Examples: ...
Never write: ...

## Time and goal
<minutes/day> | Success now = <reply / conversation / meeting>

## Search signals
<5-10 situations and phrases to look for, derived from the pain language and trigger moment>

## Not a fit
<kinds of posts/people to skip>
```

Derive "Search signals" and "Not a fit" from the answers, show them to the user, and ask them to confirm or change them.

Then update `progress.md` (stage 1 done) and tell the user the next step: finding where their clients are.
