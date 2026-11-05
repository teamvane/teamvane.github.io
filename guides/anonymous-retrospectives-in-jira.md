---
title: How to run an anonymous retrospective in Jira
description: A practical guide to sprint retrospectives where people say what they really think - anonymous cards, hidden votes, and actions that actually get done.
permalink: /guides/anonymous-retrospectives-in-jira/
---

# How to run an anonymous retrospective in Jira

**Last updated:** 5 November 2026

A retrospective only helps if people say what they really think. In many teams they don't: the newest person waits to hear what the lead thinks, nobody wants to be the one who mentions the tense release, and the same three people do all the talking. Anonymity fixes a surprising amount of that. This guide shows how to run a retrospective where cards are anonymous and votes are hidden, and how to make sure what you agree on doesn't disappear by the next sprint.

## Why anonymous?

- **People write what they'd never say out loud.** "Code reviews wait more than a day" is easy to say. "Our release process is stressful and nobody owns it" is not, unless your name isn't on it.
- **Nobody anchors on the loudest voice.** When cards appear one by one with names, people react to who wrote them, not to what they say.
- **Quieter people take part.** Writing silently first means everyone contributes, not just whoever speaks fastest.

Anonymity isn't always needed. A mature team that already trusts each other can run named retros, and seeing who wrote a card can help when you want to ask "can you tell us more?". Decide per retro, and keep the choice fixed once people start writing: cards written as anonymous must stay anonymous.

## Before the meeting

1. **Pick a format that fits the sprint.** *Went well / To improve / Ideas* works for most sprints. *Start, Stop, Continue* is good when you want concrete changes. *Mad, Sad, Glad* opens up feelings after a hard sprint. *Sailboat* (wind, anchors, rocks, island) helps a team look ahead. Change the format every few sprints so retros don't go stale.
2. **Open the board early.** Let people add cards during the sprint, as things happen. You'll get more and better cards than in five minutes of "think back over the last two weeks".
3. **Bring the facts.** Have the sprint's done and not-done work items at hand, so the conversation starts from what happened, not from memory.
4. **Check last time's actions.** Start by looking at the actions from the previous retro. If they're still open, that's the first thing to talk about.

## During the meeting

A good retrospective follows the same steps every time. Timebox each one; a timer that everyone can see helps more than a facilitator saying "two more minutes".

1. **Write (5–10 minutes).** Everyone adds cards silently. Nobody sees anyone else's cards yet, only how many there are. This is where anonymity matters most.
2. **Reveal.** Show all the cards at once, in a random order, so their order says nothing about who wrote them. Read them together.
3. **Group.** Merge cards that are about the same thing. Five cards about slow CI become one topic with five voices behind it.
4. **Vote (2–3 minutes).** Give everyone the same small number of votes, three is plenty, to put on the topics that matter most. Keep the votes hidden until everyone has voted, so people don't follow the crowd.
5. **Discuss.** Take the topics in order of votes. You'll rarely get past the top three, and that's fine: depth beats coverage.
6. **Agree on actions.** For each topic you discussed, agree on one concrete next step and who owns it. "Improve CI" is a wish. "Cache dependencies in the CI pipeline, owner: Diego, by next sprint" is an action.

## After the meeting

The most common way retrospectives fail is that actions are forgotten. Two habits prevent it:

- **Make actions real work.** Create them as Jira work items, in the same backlog as everything else, with an owner. An action that lives only in meeting notes doesn't get done.
- **Start the next retro with them.** Before writing new cards, look at what's still open. A team that sees its unfinished promises every two weeks either finishes them or decides honestly to drop them.

## Common pitfalls

- **Too many actions.** Three done actions beat ten forgotten ones. If everything is a priority, nothing is.
- **The same format every time.** People start writing the same cards. Change templates every few sprints.
- **Skipping the retro when the sprint went well.** Good sprints are exactly when you learn what to keep doing.
- **Discussing every card.** Let the votes decide. Topics nobody voted for can wait.

## Doing this with Teamvane Retrospectives

[Teamvane Retrospectives for Jira](/retrospectives/) follows exactly these steps inside a Jira space: write, reveal, group, vote, discuss and actions. Cards are anonymous by default (the app never stores who wrote an anonymous card), votes stay hidden until they're counted, and there's a timer everyone can see. It comes with 11 templates, including all the ones above. A linked sprint shows its done and not-done work items, actions become Jira work items in one click, and unfinished actions come back at the start of the next retro.

It runs on Atlassian, with no servers of our own, and it's free for teams of up to 10 users. [Get it on the Atlassian Marketplace](https://marketplace.atlassian.com/apps/2701773542/teamvane-retrospectives-for-jira).
