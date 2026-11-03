---
name: find-your-audience
description: Second stage of First Leads. Use when the user says "where are my clients", "find groups for me", "which communities should I join", "set up my channels", or when the coach finds a profile but no channels yet. Researches and proposes the specific groups, LinkedIn searches, Upwork searches and forums where the user's ideal clients ask for help, checks each place's rules, and saves the chosen list.
---

# Finding where your clients are

Use `first-leads/profile.md` to find the places where the user's ideal clients ask for help, and write `first-leads/channels.md`.

Read `${CLAUDE_PLUGIN_ROOT}/skills/first-leads/references/platform-rules.md` first.

## Steps

1. **Start from what the user already has.** Places from the profile, groups they are already in, their LinkedIn and Upwork status.

2. **Search for more**, using the ideal client and pain language:
   - **Facebook groups:** with the user's browser, search Facebook groups by the client's world (industry, role, city, stage), not by the user's service. Prefer active groups (posts in the last day) where members ask questions, over groups full of ads.
   - **LinkedIn:** build 3–5 content searches (posts) from the pain language and trigger moment, for example people posting about the problem, hiring for the role the user replaces, or asking for recommendations.
   - **Upwork** (only if the user offers remote work that fits): build 3–5 job searches from the offer and pain language. Note the user's minimum client standards (see the Upwork section in daily-leads).
   - **Forums and communities:** subreddits, professional forums, Slack/Discord communities the profile points to.

3. **Check each place** before proposing it: activity level, whether members ask for help, and the rules (self-promotion, links, DMs). Skip places whose rules forbid the kind of replies this method uses.

4. **Propose a short list.** Start small: 3–5 places in total is better than 20, but spread across **at least two different channels** (for example Facebook groups plus LinkedIn, or a forum plus Upwork), so the user never depends on a single platform. For each, show the name, why it fits, how active it is, and its key rules. Let the user choose.

5. **Joining.** If the user needs to join a group, tell them to do it themselves. Never answer group entry questions or accept terms on their behalf.

## Write channels.md

```markdown
# Channels
Updated: <date>

## Facebook groups
| Group | Link | Why it fits | Activity | Rules to remember | Rules read on |

## LinkedIn searches
| Search | What it finds |

## Upwork searches
| Search | Filters |

## Forums / communities
| Place | Link | Rules |

## Parked (try later)
...
```

Update `progress.md` (stage 2 done). Tell the user the next step: making sure their profiles are ready for the people who will check them (get-ready skill), then the daily routine of about 15–20 minutes a day.
