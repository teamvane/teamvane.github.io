---
layout: app
title: Teamvane Retrospectives for Jira
description: Guided, anonymous retrospectives inside Jira. Cards stay hidden until the reveal, votes stay hidden until they're counted, and what the team agrees becomes Jira work items that come back at the next retro.
permalink: /retrospectives/
eyebrow: For Jira Cloud · by Teamvane
app_name: Teamvane Retrospectives for Jira
tagline: Honest retros without leaving Jira. Cards stay anonymous and hidden until the reveal, the team votes on what matters, and agreed actions become work items that come back until they're done.
logo: /assets/img/retro-logo.svg
marketplace_label: Coming soon to the Atlassian Marketplace
facts:
  - Free for up to 10 users
  - Runs on Atlassian
  - Your data stays in your site
toc:
  - id: get-started
    title: Get started
  - id: how-it-works
    title: How it works
  - id: templates-and-columns
    title: Templates and columns
  - id: anonymous-or-named
    title: Anonymous or named
  - id: actions
    title: Actions
  - id: the-facilitator
    title: The facilitator
  - id: export
    title: Export
  - id: privacy-and-data
    title: Privacy and data
  - id: subscription
    title: Subscription
  - id: troubleshooting
    title: Troubleshooting
  - id: support
    title: Support
---

## Get started

1. A Jira site admin installs **Teamvane Retrospectives for Jira** from the Atlassian Marketplace. Every new site gets a free trial, and sites with up to 10 users can use it for free.
2. Open a space and click **Retrospectives** in its navigation (it may be under **More**).
3. Click **New retrospective**. Optionally link a **sprint**, pick a **template**, choose how many **votes per person**, and whether cards are **anonymous** (on by default). Then click **Create**.

Whoever creates a retrospective is its **facilitator**: they move everyone from one step to the next. Anyone who can browse the space can join; just open the retrospective from the list.

## How it works

A retrospective goes through six steps, shown at the top of the page. Only the facilitator moves it forward; everyone else follows along live.

1. **Write.** Everyone adds cards to the columns. **Nobody sees anyone else's cards**, only how many have been written so far. You can edit or delete your own cards. The retrospective can stay open for days, so people can add cards during the sprint.
2. **Reveal.** The facilitator clicks **Reveal cards**. Everyone now sees every card, in a random order that says nothing about who wrote what. Cards can't be hidden again, and no more can be added.
3. **Group.** Put cards that are about the same thing together: click **Move** on a card, then **Merge here** on the card to group it with. **Move group** moves a whole group; **Ungroup** takes a card out of its group; **Cancel** puts a card back.
4. **Vote.** Everyone gets a number of votes (3 by default) to put on the groups and cards that matter most, several on one card if you like. **Votes stay hidden** until the facilitator clicks **Count votes**; you only see how many people have voted.
5. **Discuss.** Groups and cards are listed with the most votes first. Talk them through, and click **Add action** on a card to note what the team will do about it.
6. **Actions.** Agree on the actions and turn them into Jira work items (see [Actions](#actions)). Then the facilitator clicks **End retrospective**.

**Timer.** The facilitator can start a countdown for any step (**Timer**). When it runs out, everyone with the retrospective open gets a "Time's up" notification.

**Who's here.** The avatars under **Here now** show who has the retrospective open.

**Linked sprint.** If the retrospective is linked to a sprint, the Write and Reveal steps show how many work items were done and which ones weren't.

**Still open from earlier retros.** Actions from the space's earlier retrospectives that aren't done yet appear at the start of each new one, with their live status, so the team begins by checking what it promised last time.

## Templates and columns

Pick a template when you create a retrospective. Each one comes with its columns, colors and a short hint under each column title:

- **Went well / To improve / Ideas**
- **Start, Stop, Continue**
- **Mad, Sad, Glad**
- **4Ls**: Liked, Learned, Lacked, Longed for
- **Went well / Less well / Try next / Puzzles**
- **Keep, Add, Less, More**
- **Drop, Add, Keep, Improve**
- **Starfish**: Keep doing, Less of, More of, Stop doing, Start doing
- **Rose, Thorn, Bud**
- **Plus / Delta**
- **Sailboat**: Wind, Anchors, Rocks, Island

During the Write step, the facilitator can rename, recolor, add and remove columns in **Settings** (up to 6). A column that already has cards can't be removed.

## Anonymous or named

You choose when you create a retrospective, and it can't be changed afterwards.

- **Anonymous** (the default): the app never stores who wrote a card. While the retrospective is open it keeps a scrambled code that lets you edit your own cards; when the retrospective ends, that code is deleted for good, so nobody, not even Teamvane, can work out who wrote what.
- **Named**: after the reveal, each card shows who wrote it.

In both cases, votes are never stored against anyone's name, and the export never includes authors.

## Actions

Anyone can add actions during Discuss and Actions. Each action can be:

- **plain text**, ticked off by hand when it's done;
- turned into a new work item with **Create work item**: choose the work type and, optionally, an assignee. It's created as you, so Jira's own permissions apply;
- linked to an existing work item with **Link existing** (type its key, for example TEAM-12). Linked actions are done when their work item is done.

Following actions up (creating or linking work items, ticking them off) still works after the retrospective has ended.

## The facilitator

Only the facilitator can move between steps, set the timer, change the settings, end or delete the retrospective. If the facilitator leaves, anyone in the retrospective can click **Take over** next to their name.

Going back is possible where nothing is lost: from Group to Reveal, from Vote to Group (the votes cast so far are discarded), and from Actions to Discuss.

The facilitator and the space's admins can delete a retrospective from the list.

## Export

Once the cards are revealed, **Export** shows the retrospective as **Markdown** (to paste into a Confluence page, a chat or an email) and as **CSV** (to paste into a spreadsheet). Exports never include who wrote a card.

## Privacy and data

- Cards are hidden until the reveal and votes until they're counted. This is enforced on the server, not just hidden on screen.
- The app runs entirely on Atlassian's platform ("Runs on Atlassian") and keeps its data in your site, following your site's data residency.
- It stores only account ids (the facilitator's, and card authors' in named retrospectives), never names or pictures.
- Retrospectives are deleted automatically 12 months after they end.
- "Here now" is shared with people who have the same retrospective open: an account id, nothing else.

Details: [Privacy Policy](/retrospectives/privacy/) · [Terms of Use](/retrospectives/terms/) · [Data Processing Addendum](/retrospectives/dpa/) · [Security](/security/)

## Subscription

Sites with up to 10 users can use the app for free. Larger sites get a free trial, then a subscription through the Atlassian Marketplace. If a site has no active subscription or trial, the app shows **"Retrospectives needs a subscription"**. Ask a Jira admin to start one.

## Troubleshooting

**I can't find Retrospectives in my space.** Look in the space's navigation, or under **More**. You need permission to browse the space.

**Someone sees something different from everyone else.** After an app update, Jira keeps the version that was loaded when the page opened. Reload the page.

**No sprints to choose from.** Only spaces with a scrum board have sprints. The sprint list shows the active sprints and the most recent closed ones.

**"Create work item" fails.** Jira explains why in the message: usually the work type needs other required fields, or the assignee can't be assigned in this space. Create it in Jira and use **Link existing** instead.

## Support

Email **support@teamvane.com**, in English, French or Spanish. We reply within one business day.
