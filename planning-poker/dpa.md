---
title: Data Processing Addendum – Teamvane Planning Poker for Jira
permalink: /planning-poker/dpa/
---

<!--
DRAFT for review. Fill [DATE] with the publication date before publishing.
Not legal advice: have it reviewed before publishing.
-->

# Data Processing Addendum – Teamvane Planning Poker for Jira

**Last updated:** [DATE]

This Data Processing Addendum ("DPA") is part of the [Terms of Use](/planning-poker/terms/) of **Teamvane Planning Poker for Jira** ("the Product"). It applies when the Product processes personal data on behalf of the customer that installed it ("Customer"), as required by article 28 of the EU General Data Protection Regulation ("GDPR").

## 1. Roles

- The **Customer** is the controller.
- **Teamvane**, the trading name of Alexandre Blasco Brasó, based in France ("Teamvane"), is the processor.

## 2. Standard Contractual Clauses

The Customer and Teamvane agree to the **standard contractual clauses between controllers and processors** adopted by the European Commission in [Implementing Decision (EU) 2021/915](https://eur-lex.europa.eu/eli/dec_impl/2021/915/oj) (the "Clauses"). The Clauses are incorporated into this DPA by reference, with these choices:

- **Clause 5 (docking clause):** not used.
- **Clause 7.7 (use of sub-processors):** Option 2, general written authorisation. Teamvane will tell the Customer about any intended addition or replacement of a sub-processor at least **30 days** in advance. It will email the Customer's technical contact and update Annex IV on this page, so the Customer can object before the change.
- **Annexes I to IV:** as set out below.

If this DPA or the Terms of Use conflict with the Clauses, the Clauses prevail.

## 3. Additional terms

These terms add to the Clauses without contradicting them.

1. **Instructions.** The Customer instructs Teamvane to process personal data to provide the Product, as described in Annex II. Installing and using the Product, and configuring it in Jira, are the Customer's documented instructions.
2. **Atlassian's platform and transfers.** The Product runs on Atlassian's Forge platform. The Customer instructs Teamvane to use it, including any transfers of personal data Atlassian makes under its [Forge Data Processing Addendum](https://developer.atlassian.com/platform/forge/resources/Forge-Data-Processing-Addendum.pdf). Teamvane itself is established in the European Union.
3. **Personal data breaches.** Teamvane will notify the Customer without undue delay after becoming aware of a breach affecting the Customer's personal data, and where possible within 48 hours.
4. **Requests from individuals.** Data in the Product can be removed by ending a session, and all of it by uninstalling the Product. Teamvane will help the Customer answer other requests. Write to support@teamvane.com.
5. **Information and audits.** Teamvane will first answer audit requests in writing and with documentation. The Product has no servers or premises of its own: all processing happens on Atlassian's infrastructure, which Atlassian audits under its own certifications.
6. **End of processing.** Personal data is deleted automatically as described in Annex II. When the Product is uninstalled, Atlassian deletes the Product's stored data after 28 days.

---

## Annex I – List of parties

**Controller:** the Customer, as identified by its Atlassian Marketplace licence for the Product. Contact: the technical contact the Customer gave Atlassian.

**Processor:** Teamvane (Alexandre Blasco Brasó), France. Contact: support@teamvane.com.

## Annex II – Description of the processing

| | |
| --- | --- |
| **Data subjects** | People in the Customer's Jira site who use the Product: participants, facilitators and people who save estimates |
| **Personal data** | Atlassian account ID, display name and profile picture address, the cards each person plays, and while the Product is open, the ID of the issue a person is viewing and whether they are "just watching" |
| **Sensitive data** | None |
| **Nature of the processing** | Storing, showing and sending to other participants in real time; reading Jira data with the acting user's permissions; writing an agreed estimate to a Jira field when a user saves it; reporting stored account IDs to Atlassian daily, as Atlassian requires; automatic deletion |
| **Purpose** | Running planning poker sessions in the Customer's Jira site |
| **Duration** | Votes: until the next round or the end of the session. Session data, including round history: 72 hours after the last start, reveal or new round, or until the session is ended. Presence messages: not stored, held by Atlassian's Realtime service for less than a minute. All stored data: deleted 28 days after uninstallation. |
| **Processing by sub-processors** | Atlassian hosts and runs the Product, stores its data and delivers its live updates and logs (see Annex IV) |

## Annex III – Technical and organisational measures

- **Hosting:** the Product runs and stores data only on Atlassian's Forge platform. Atlassian encrypts stored data on disk and keeps it in the same location as the Customer's Jira site.
- **Access control:** every action is checked on the server against the acting user's own Jira permissions. Live session updates reach only browsers that passed that check, and browsers cannot publish votes or reveals.
- **Vote privacy:** while a round is open, the server never sends anyone's card to a browser.
- **Data minimisation:** the Product stores only what a session needs and deletes it automatically (see Annex II), with a daily job removing any expired leftovers. Issue details are read when needed and not stored.
- **Closed and changed accounts:** every day the Product reports the accounts it holds data about to Atlassian. It erases the data of accounts Atlassian reports as closed, and refreshes or erases the data of accounts reported as changed.
- **Least privilege:** the Product requests only the Atlassian permission scopes it needs.
- **Teamvane's own access:** Teamvane has no tool to browse the data stored in the Customer's site. It can read the Product's error logs while the Customer's admins allow log sharing (Atlassian Administration → Connected apps → the Product → Logs access). Teamvane's accounts use two-step verification.
- **Testing:** automated tests check the privacy and permission rules before each release.

## Annex IV – List of sub-processors

| Sub-processor | What it does | Location |
| --- | --- | --- |
| Atlassian (Atlassian Pty Ltd and its affiliates) | Runs the Product on the Forge platform, stores its data, delivers live updates and keeps logs | The same location as the Customer's Jira site data. Atlassian's own sub-processors are listed on [atlassian.com](https://www.atlassian.com/legal/sub-processors). |
