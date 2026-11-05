---
title: How to run planning poker in Jira without anchoring
description: A practical guide to estimating with planning poker in Jira - hidden votes, a good refinement rhythm, and saving the agreed estimate where your team works.
permalink: /guides/planning-poker-in-jira/
---

# How to run planning poker in Jira without anchoring

**Last updated:** 5 November 2026

Planning poker is a simple way for a team to estimate work together: everyone picks a card with their estimate, all the cards are shown at the same moment, and the team talks about the differences. The magic is in that "same moment". This guide explains why, and how to run estimation sessions in Jira that are quick, fair and actually useful.

## Why the votes must stay hidden

If one person says "that's a 3" before everyone else has decided, the rest of the team drifts towards 3. That's **anchoring**, and it happens even when nobody means it to: the senior developer thinks out loud, the product owner looks hopeful, or someone simply votes first where everyone can see.

Hidden votes prevent it. Each person decides on their own, and only then are the cards revealed together. When the estimates differ, that's not a problem to hide; it's the most useful part of the session. The person who picked 8 when everyone else picked 3 often knows something the others don't.

## Before the session

1. **Refine first, estimate second.** An issue nobody understands can't be estimated. Make sure each issue has a clear description and acceptance criteria before it reaches the session.
2. **Pick a deck and stick to it.** The Fibonacci-style deck (1, 2, 3, 5, 8, 13…) is the most common: the growing gaps reflect that big work is less certain. T-shirt sizes (XS to XL) suit rough, early estimates.
3. **Decide who votes.** The people who will do the work vote. Product owners and managers usually listen and answer questions, but don't estimate.
4. **Prepare a queue.** List the issues you want to estimate, in order, so the session moves from one to the next without hunting through the backlog.

## Running a round

1. **Read the issue together** and let people ask questions. Keep it short; this isn't the place to design the solution.
2. **Everyone picks a card, privately.** You should be able to see who has voted, so you know who you're waiting for, but never what they voted.
3. **Reveal all the cards at once.**
4. **If everyone agrees,** you're done. Save the estimate and move on.
5. **If the cards are far apart,** ask the highest and the lowest voter to explain their thinking. Then vote again. Two rounds are usually enough.
6. **Agree on the estimate** and save it to the issue straight away, so it doesn't get lost in meeting notes.

## Tips for a good session

- **Don't average the cards.** If two people say 3 and two say 13, the answer isn't 8: it's a conversation about what the 13s see.
- **Big numbers mean "split it".** If an issue keeps landing on 13 or more, it's probably several issues. Split it rather than argue about the number.
- **Timebox.** A few minutes per issue is plenty. If an issue needs more, it needs more refinement first, not more estimating.
- **Use a "?" or "coffee" card.** It's fine to say "I don't know enough to estimate this". That's useful information.
- **Estimate relative to past work.** "Is this bigger or smaller than the CSV export we did last sprint?" is easier to answer than "how many days?".

## Saving estimates in Jira

Estimates belong on the issue, in the field your team plans with: usually *Story points*, sometimes a separate field per role (for example a development estimate and a QA estimate). Saving them during the session, not afterwards, means the backlog is ready for sprint planning the moment the meeting ends.

## Doing this with Teamvane Planning Poker

[Teamvane Planning Poker for Jira](/planning-poker/) brings exactly this into Jira. Votes stay hidden until the reveal, and that's enforced on the server, not just hidden on screen. You can see who's here and who has voted, and when everyone has voted the cards turn after a short countdown that anyone can hold. On a space's Planning Poker page you build an estimation queue from your backlog, sprints or a search, and the team moves from issue to issue together. The agreed estimate saves to story points, or any number field your space uses, in one click.

It runs on Atlassian, with no servers of our own, and it's free for teams of up to 10 users. [Get it on the Atlassian Marketplace](https://marketplace.atlassian.com/apps/2939883696/teamvane-planning-poker-for-jira).

*Planning Poker® is a registered trademark of Mountain Goat Software, LLC. Teamvane is not affiliated with Mountain Goat Software.*
