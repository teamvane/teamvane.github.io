---
title: Privacy Policy – Teamvane Retrospectives for Jira
permalink: /retrospectives/privacy/
---

# Privacy Policy – Teamvane Retrospectives for Jira

**Last updated:** 20 October 2026

This policy explains what personal data the **Teamvane Retrospectives for Jira** app ("the app") handles, why, where it is kept and for how long. It applies to the app as installed from the Atlassian Marketplace.

## Who we are

Teamvane is the trading name of Alexandre Blasco Brasó, based in France ("Teamvane", "we", "us"). You can reach us at **support@teamvane.com**.

## The short version

- The app runs entirely on Atlassian's Forge platform. Teamvane has no servers or databases of its own, and the app sends nothing outside Atlassian.
- The app keeps what a retrospective needs: its cards, votes and actions, and the Atlassian account IDs of the facilitator and, in named retrospectives only, of each card's author. It never stores names or profile pictures.
- In **anonymous** retrospectives (the default), the app never stores who wrote a card. When the retrospective ends, even the scrambled code that let people edit their own cards is deleted, so nobody, not even Teamvane, can work out who wrote what.
- Cards are not sent to anyone else's browser until the reveal, and nobody's votes are ever sent to anyone else: each person sees only their own, and everyone sees the totals once counted.
- Retrospectives are deleted automatically **12 months** after they end, or earlier if the facilitator or a space admin deletes them.
- The app writes to Jira only when someone creates a work item for an action, and as that person.
- No cookies, no analytics, no advertising, no tracking. We never sell data.

## Where the app runs

The app is built on [Atlassian Forge](https://developer.atlassian.com/platform/forge/) and "Runs on Atlassian". Its code runs on Atlassian's infrastructure, and its data is kept in Atlassian's Forge hosted storage, inside your Atlassian site's installation of the app. Atlassian keeps this data in the same location as your Jira site's data, so it follows your site's data residency, and encrypts it on disk.

We have no tool to browse the data the app stores in your site.

## What the app stores

| Data | Why | How long |
| --- | --- | --- |
| **Retrospective:** name, linked sprint (ID and name), columns, settings, current step, timer, the **facilitator's account ID**, vote totals, and while it is open, a random secret used for anonymous ownership (see below) | To run the retrospective | 12 months after it ends, or after its last change if it never ends. The secret is deleted when it ends. |
| **Cards:** column, text, group, and in **named** retrospectives the **author's account ID**. While the retrospective is open, each card also has an *owner tag* (see below) | To show the board and let people edit their own cards | Same as the retrospective. Owner tags are deleted when it ends. |
| **Votes:** how many votes went to each card, stored under the voter's owner tag, never their account ID | To count the votes | Only while voting is open. Once counted, only the totals remain. |
| **Actions:** text, done or not, and the ID and key of a linked Jira work item | To follow up on what the team agreed | Same as the retrospective |
| **A record of which accounts each retrospective holds data about** | For the daily report to Atlassian (see below) | Same as the retrospective |

**Card and action text** is written by the people taking part. It may mention people or contain other personal data if someone chooses to write it; your organisation decides what is appropriate to write.

**Anonymous ownership.** While an anonymous retrospective is open, each card stores a code made from a random secret and the writer's account ID with a one-way function (HMAC-SHA256). The app can tell you which cards are yours without storing who you are, and the code alone says nothing about anyone. When the retrospective ends, the secret and every code are deleted.

Names and profile pictures are never stored: the page shows people with Atlassian's own user component, which loads them from Atlassian when the page opens.

If your site uninstalls the app, Atlassian keeps the app's stored data for 28 days and then deletes it.

## When an Atlassian account is closed

Once a day, as Atlassian requires, the app tells Atlassian which accounts it holds data about, and Atlassian answers which of them have been closed. For **closed accounts**, the app removes their account ID: a retrospective they facilitated no longer has a facilitator (anyone taking part may then lead it), and their cards stay, shown as written by a "Former user". Because the app stores no names or pictures, there is nothing to update when an account is changed.

## What the app reads from Jira without keeping it

To work, the app reads the following from Jira at the time it's needed, **with the permissions of the person using it**:

- Whether you can browse the space and whether you administer it, to decide what you may see and do.
- The space's boards and sprints, to offer a sprint to link.
- The linked sprint's work items (key, summary and status), to show what was done and not done.
- The work types you can create in the space, and the key, summary and status of work items linked to actions.

This information is shown in your browser and is not stored by the app, except for the IDs and names listed in the table above.

## What the app writes to Jira

When someone clicks **Create work item** on an action, the app creates a work item in the space with the action's text as its summary, a short description naming the retrospective, and the assignee they chose. It does so as the person creating it, so Jira's own permissions apply and Jira records them as its creator. The app writes nothing else to Jira.

## Live updates

The app uses Atlassian's Forge Realtime service to update everyone's screen live:

- **Change notices** go to people with the space's Retrospectives page open. They contain the retrospective's ID and, at most, how many cards have been written or how many people have voted, never a card's text or anyone's votes.
- **Presence** ("Here now") is shared between the browsers of people with the same retrospective open. Each message contains the retrospective's ID and a person's account ID. Realtime keeps these messages for less than a minute, so people who join late can catch up, and the app never stores them.

## In your browser

- The app stores nothing in your browser.
- The app sets no cookies and includes no analytics, advertising or tracking code.
- The "Time's up" notification is shown by Jira.

## Error logs

When something goes wrong, the app writes a technical error message to its logs. It never logs card text, action text or account IDs on purpose. Atlassian collects these logs and, while log sharing is on, lets us read up to the last 60 days of them so we can fix problems. Log sharing is on by default. Your organisation's admins can turn it off in Atlassian Administration, under **Connected apps**, in the app's **Details** tab (**Logs access**).

## Information we receive as the app's provider

- **Licence information.** When your organisation installs or buys the app, Atlassian shares licence details with us. These can include your organisation's name and country, and the name and email address of the technical and billing contacts your organisation gave Atlassian. We use them to manage licences and contact you about the app.
- **Support requests.** If you email us, we receive your name, email address and whatever you choose to send. We use it to help you. Our email is hosted by Google.

## Our role under the GDPR

- For the data the app stores in your site, **your organisation is the controller** and **Teamvane is a processor** acting on your organisation's behalf. Atlassian hosts this data as our sub-processor under its [Forge Data Processing Addendum](https://developer.atlassian.com/platform/forge/resources/Forge-Data-Processing-Addendum.pdf). Our [Data Processing Addendum](/retrospectives/dpa/) sets out the terms.
- For licence information and support requests, **Teamvane is the controller**. We process them to provide the app and support you (performing our contract with your organisation), out of our legitimate interest in managing our customers, and to meet our accounting and tax obligations.

## Who we share data with

- **Atlassian**, which hosts the app, runs the Marketplace and handles purchases.
- **Google**, which hosts our support email.
- Authorities, only when the law requires it.

We don't sell personal data or share it for advertising.

## International transfers

The app's stored data follows your Jira site's location. Atlassian and Google may process data in other countries, including outside the European Economic Area. They protect such transfers with the safeguards in their data processing terms, such as the EU Standard Contractual Clauses.

## How long we keep our own records

- Support emails: up to 3 years after our last exchange.
- Licence and payment records: as long as French accounting and tax law requires.

## Security

- The app runs and stores its data only on Atlassian's infrastructure.
- Every action is checked on the server against the user's own Jira permissions: only people who can browse a space can see or change its retrospectives.
- Before the reveal, the server never sends a card to anyone but its writer, and it never sends one person's votes to anyone else.
- See also [Security](/security/).

## Your rights

Under the GDPR you have the right to access, correct or delete your personal data, to restrict or object to its processing, and to data portability.

For data the app stores in your Jira site, please contact your organisation's Jira admin first, since your organisation controls it. We will help them answer your request. You can also email us at support@teamvane.com. Note that in anonymous retrospectives, nobody can tell which cards are yours once the retrospective has ended.

You can complain to the French data protection authority, the [CNIL](https://www.cnil.fr/), or to the authority in your country.

## Children

The app is a workplace tool and is not meant for children under 16.

## Changes to this policy

We will update this page when the app's data handling changes, and change the "Last updated" date. For significant changes, we will also say so in the app's Marketplace listing.

## Contact

Teamvane, Alexandre Blasco Brasó – **support@teamvane.com**
