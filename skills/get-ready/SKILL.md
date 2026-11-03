---
name: get-ready
description: Readiness stage of First Leads, before the daily routine. Use when the user says "check my profiles", "am I ready", "I have nothing to show", "help me with my portfolio", "write my LinkedIn headline", "how do I get testimonials", or when the coach finds no readiness check yet. Makes sure that when a good comment works and someone opens the user's profile, they understand in seconds what the user does, see proof, and know how to get in touch.
---

# Get ready to be checked

When a comment or proposal works, the next thing the person does is open the user's profile. If it is empty or unclear, the lead is lost silently. This stage makes sure the user is ready before the daily routine starts.

Read `first-leads/profile.md` and `first-leads/channels.md` first. As in every stage, the user makes every change on their own accounts; you check and draft.

## 1. The ten-second check

With the user's browser, open their public profiles on the channels in `channels.md` (Facebook profile and/or page, LinkedIn, Upwork). For each, answer from a stranger's point of view:
- Is it clear within ten seconds what they do, and for whom?
- Is there proof (work, example, before/after, testimonial)?
- Is there one clear way to make contact, allowed by the platform?

Report in a short table: channel, what works, what is missing.

## 2. Headline and About

Draft, in the user's voice and in their clients' words (from the pain language in the profile):
- A headline: who they help, with what. No list of titles, no buzzwords.
- A short About: the problem clients come with, how the user helps, one line of proof, how to reach them.
- For Upwork: title and overview that answer what clients search for. No contact details (platform rule).

The user edits and updates the profiles themselves.

## 3. Proof: at least one, ideally three

Match the proof to the goal in the profile (see `${CLAUDE_PLUGIN_ROOT}/skills/first-leads/references/goals.md`): work and testimonials for clients; a demo and a clear pilot offer for pilot partners and early users; a partner one-pager for collaborations. The rest of this section is written for clients; adapt it the same way.

Every young business needs something to show. Aim for **at least one piece of proof before the daily routine starts, and three as the goal**.

Proof can be:
- A real piece of work, with the client's permission.
- An example or demo made specifically to show what the user can do.
- A before/after.
- A testimonial: a few sentences from a client, in their words, with their name if they agree.

**If the user has nothing**, help them build it:
- **A sample project:** pick a typical client problem from the profile and create a small, real example of solving it (for a designer, a redesign of a public example; for a consultant, a short teardown of a common process; for a developer, a small working demo).
- **Volunteer work (pro bono):** suggest offering the service for free to 1–3 suitable businesses or nonprofits, to get real results and testimonials. Set it up properly:
  - A small, defined scope and a time limit (for example, two weeks, one deliverable).
  - Agreed in advance: in exchange, a short testimonial and permission to show the work (or an anonymized version).
  - Choose recipients who look like the paying clients the user wants, so the proof speaks to the right audience.
  - Treat it like paid work: clear start, clear end, a short summary of results.
- Draft the message the user sends to offer the volunteer work: short, specific about what they will do and what they ask in return. The user sends it.

## 4. One link that holds it all: a simple landing page

Build the user a one-page landing page from what you already have (the profile and the proof). It is also part of spreading the risk: if a platform account is lost, the page and the people who reached the user through it stay.

**Structure (one page, nothing more):**
1. Who I help and with what, in the clients' own words (one line, big).
2. The problem they come with, and how the user solves it (3–4 short lines).
3. Proof: the 1–3 pieces from step 3 (samples, before/after, testimonials).
4. How it works with the user (2–4 simple steps).
5. One way to get in touch: a form, WhatsApp click-to-chat link (`https://wa.me/<number>`), or email. One, not five.

**Rules:**
- The goal: someone arriving from a comment understands in ten seconds and knows how to reach out. Cut everything else.
- Real content only: no invented clients, numbers or testimonials.
- Mobile first: most visitors come from a phone.
- Write it in the language of the user's clients.

**Build:** create a single self-contained HTML file (inline CSS, no external dependencies, readable on mobile) in the `first-leads` folder, and show it to the user. Iterate on wording with them.

**Publish:** guide the user step by step to put it online for free; the user does every click and sign-up:
- GitHub Pages (a free account; upload the file as `index.html` in a public repository, then enable Pages in Settings), or
- Google Sites (paste the text and images into a one-page site), or
- a page builder the user already has.

If they own a domain, explain how to connect it, or point them to their provider's help page.

**Where to use the link:** in the Facebook profile/page, LinkedIn Featured and contact info, and in comments only where the group rules allow links and the person asked. **Not on Upwork before a contract** (platform rule: no external contact details); there, use the Upwork portfolio instead.

## Finish

Record in `progress.md`: readiness check done, proof count (x of 3), what is still missing. The daily routine can start with one piece of proof; keep working toward three in parallel, and remind the user in weekly reviews until there are three.
