---
title: Privacy Policy – Teamvane Planning Poker for Jira
permalink: /planning-poker/privacy/
---

# Privacy Policy – Teamvane Planning Poker for Jira

**Last updated:** 13 October 2026

This policy explains what personal data the **Teamvane Planning Poker for Jira** app ("the app") handles, why, where it is kept and for how long. It applies to the app as installed from the Atlassian Marketplace.

## Who we are

Teamvane is the trading name of Alexandre Blasco Brasó, based in France ("Teamvane", "we", "us"). You can reach us at **support@teamvane.com**.

## The short version

- The app runs entirely on Atlassian's Forge platform. Teamvane has no servers or databases of its own, and the app sends nothing outside Atlassian.
- The app keeps only what a planning poker session needs: who is taking part (Atlassian account ID, display name and profile picture address) and the cards they play.
- Session data is deleted automatically **72 hours** after the last start, reveal or new round on an issue, or straight away when someone ends the session.
- While a round is open, nobody's card is sent to anyone's browser. Cards are shared only at the reveal.
- The app writes to Jira only when someone saves an estimate, only to the field the space chose, and as that person.
- No cookies, no analytics, no advertising, no tracking. We never sell data.

## Where the app runs

The app is built on [Atlassian Forge](https://developer.atlassian.com/platform/forge/) and "Runs on Atlassian". Its code runs on Atlassian's infrastructure, and its data is kept in Atlassian's Forge hosted storage, inside your Atlassian site's installation of the app. Atlassian keeps this data in the same location as your Jira site's data, so it follows your site's data residency, and encrypts it on disk.

We have no tool to browse the data the app stores in your site.

## What the app stores

| Data | Why | How long |
| --- | --- | --- |
| **Votes:** account ID, display name, profile picture address and the card played | To show who has voted and, at the reveal, what everyone played | Until the next round starts or the session ends. In any case, no longer than the session (see the next row). |
| **Session:** deck, round number, whether cards are revealed, the facilitator (account ID and display name), round history (account ID, display name and card for each revealed round, up to 20 rounds), the estimation fields being estimated and the last value saved | To run the session and show earlier rounds | 72 hours after the last start, reveal or new round on that issue. Deleted straight away when someone ends the session. |
| **Refinement page's current issue:** an issue ID | So everyone on the refinement page looks at the same issue | 72 hours |
| **Space defaults:** the chosen deck and whether sessions are led | So starting a session is one click | Until changed |
| **Estimation queue:** issue IDs | The list of issues the team plans to estimate | Until changed |
| **Estimation fields:** Jira field IDs and names | Which fields estimates are saved to | Until changed, if chosen by a space admin. 7 days if detected automatically. |

Only the first two rows contain personal data. The app stops using data the moment it expires, and once a day it deletes any expired data Atlassian hasn't removed yet.

If your site uninstalls the app, Atlassian keeps the app's stored data for 28 days and then deletes it.

## When an Atlassian account is closed or changes

Once a day, as Atlassian requires, the app tells Atlassian which accounts it holds data about, and Atlassian answers which of them have been closed or changed:

- **Closed accounts** are erased: their votes are deleted, and their name and account ID are removed from round history and from leading a session. Their cards stay in round history, shown as "Former user", so earlier rounds still add up.
- **Changed accounts** get their stored name and profile picture updated from Jira. If Jira no longer shows the profile, they are erased instead.

## What the app reads from Jira without keeping it

To work, the app reads the following from Jira at the time it's needed, **with the permissions of the person using it**:

- Your account ID, display name and profile picture, to show you in a session.
- Issue details (key, summary, status, type, project and current estimate) for the issue panel and the refinement page.
- The number fields used in a space, to offer them as estimation fields.
- Whether you administer a space, to decide who may change the space's estimation fields.

This information is shown in your browser and is not stored by the app, except for the IDs listed in the table above.

## What the app writes to Jira

When someone clicks **Save** after a reveal, the app writes the chosen estimate to the space's chosen estimation field on that issue. It does so as the person saving, so Jira's own edit permissions apply, and Jira records the change in the issue's history under that person's name. The app writes nothing else to Jira.

## Live updates

The app uses Atlassian's Forge Realtime service to update everyone's screen live:

- **Session updates** (someone has voted, the reveal, new rounds, saved estimates) go only to people viewing that issue who have access to it.
- **Presence** ("who's here", "just watching") is shared between the browsers of everyone with the app open in the same Jira space. Each message contains a person's account ID, display name, profile picture address, the ID of the issue they're on and whether they're just watching. It never contains a card or an issue title. Realtime keeps these messages for less than a minute, so people who join late can catch up, and they are never stored by the app.

## In your browser

- If you choose **Just watching**, the app remembers that choice in your browser's local storage. Nothing else is stored in your browser.
- The app sets no cookies and includes no analytics, advertising or tracking code.
- Profile pictures are loaded from the image address Atlassian provides for each account.

## Error logs

When something goes wrong, the app writes a technical error message to its logs. Atlassian collects these logs and, while log sharing is on, lets us read up to the last 60 days of them so we can fix problems. Log sharing is on by default. Your organisation's admins can turn it off in Atlassian Administration, under **Connected apps**, in the app's **Details** tab (**Logs access**).

## Information we receive as the app's provider

- **Licence information.** When your organisation installs or buys the app, Atlassian shares licence details with us. These can include your organisation's name and country, and the name and email address of the technical and billing contacts your organisation gave Atlassian. We use them to manage licences and contact you about the app.
- **Support requests.** If you email us, we receive your name, email address and whatever you choose to send. We use it to help you. Our email is hosted by Google (Gmail).

## Our role under the GDPR

- For the data the app stores in your site, **your organisation is the controller** and **Teamvane is a processor** acting on your organisation's behalf. Atlassian hosts this data as our sub-processor under its [Forge Data Processing Addendum](https://developer.atlassian.com/platform/forge/resources/Forge-Data-Processing-Addendum.pdf). Our [Data Processing Addendum](/planning-poker/dpa/) sets out the terms.
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
- Every action is checked on the server against the user's own Jira permissions.
- While a round is open, the server never sends anyone's card to a browser.
- Session updates reach only browsers that passed the access check for that issue, and browsers cannot publish fake votes or reveals.

## Your rights

Under the GDPR you have the right to access, correct or delete your personal data, to restrict or object to its processing, and to data portability.

For data the app stores in your Jira site, please contact your organisation's Jira admin first, since your organisation controls it. We will help them answer your request. You can also email us at support@teamvane.com.

You can complain to the French data protection authority, the [CNIL](https://www.cnil.fr/), or to the authority in your country.

## Children

The app is a workplace tool and is not meant for children under 16.

## Changes to this policy

We will update this page when the app's data handling changes, and change the "Last updated" date. For significant changes, we will also say so in the app's Marketplace listing.

## Contact

Teamvane, Alexandre Blasco Brasó – **support@teamvane.com**
