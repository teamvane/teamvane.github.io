---
title: Data Processing Addendum – Teamvane Retrospectives for Jira
permalink: /retrospectives/dpa/
---

# Data Processing Addendum – Teamvane Retrospectives for Jira

**Last updated:** 20 October 2026

This Data Processing Addendum ("DPA") is part of the [Terms of Use](/retrospectives/terms/) of **Teamvane Retrospectives for Jira** ("the Product"). It applies when the Product processes personal data on behalf of the customer that installed it ("Customer"), as required by article 28 of the EU General Data Protection Regulation ("GDPR").

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
4. **Requests from individuals.** A retrospective and everything in it can be deleted by its facilitator or a space admin, and all of the Product's data by uninstalling the Product. In anonymous retrospectives, cards cannot be linked to their writers once the retrospective has ended. Teamvane will help the Customer answer other requests. Write to support@teamvane.com.
5. **Information and audits.** Teamvane will first answer audit requests in writing and with documentation. The Product has no servers or premises of its own: all processing happens on Atlassian's infrastructure, which Atlassian audits under its own certifications.
6. **End of processing.** Personal data is deleted automatically as described in Annex II. When the Product is uninstalled, Atlassian deletes the Product's stored data after 28 days.

---

## Annex I – List of parties

**Controller:** the Customer, as identified by its Atlassian Marketplace licence for the Product. Contact: the technical contact the Customer gave Atlassian.

**Processor:** Teamvane (Alexandre Blasco Brasó), France. Contact: support@teamvane.com.

## Annex II – Description of the processing

| | |
| --- | --- |
| **Data subjects** | People in the Customer's Jira site who use the Product: facilitators, people writing cards and voting, and people adding actions; and anyone mentioned in what they write |
| **Personal data** | Atlassian account IDs of facilitators, and of card authors in named retrospectives; pseudonymous owner codes (HMAC of the account ID with a per-retrospective secret) for cards and votes while a retrospective is open; card and action text written by users, which may contain personal data; while the Product is open, the account ID and retrospective ID of people present |
| **Sensitive data** | None intended. Users may write free text; the Customer decides what is appropriate. |
| **Nature of the processing** | Storing, showing and sending to other participants in real time; reading Jira data with the acting user's permissions; creating a Jira work item for an action when a user asks; reporting stored account IDs to Atlassian daily, as Atlassian requires; automatic deletion |
| **Purpose** | Running team retrospectives in the Customer's Jira site |
| **Duration** | Retrospectives, with their cards and actions: 12 months after they end (or after their last change, if never ended), or until deleted. Owner codes and the per-retrospective secret: until the retrospective ends. Individual votes: until the votes are counted. Presence messages: not stored, held by Atlassian's Realtime service for less than a minute. All stored data: deleted 28 days after uninstallation. |
| **Processing by sub-processors** | Atlassian hosts and runs the Product, stores its data and delivers its live updates and logs (see Annex IV) |

## Annex III – Technical and organisational measures

- **Hosting:** the Product runs and stores data only on Atlassian's Forge platform. Atlassian encrypts stored data on disk and keeps it in the same location as the Customer's Jira site.
- **Access control:** every action is checked on the server against the acting user's own Jira permissions; only users who can browse a space can see or change its retrospectives.
- **Confidentiality of cards and votes:** before the reveal, the server never sends a card to anyone but its writer. One person's votes are never sent to anyone else, and are deleted once counted.
- **Pseudonymisation and anonymisation:** in anonymous retrospectives, card authors are never stored. Ownership uses one-way codes made with a per-retrospective secret; the secret and the codes are deleted when the retrospective ends.
- **Data minimisation:** the Product stores account IDs only where needed and never names or profile pictures. Jira data is read when needed and not stored, except for the IDs listed in Annex II. Exports never include authors.
- **Storage limitation:** retrospectives are deleted automatically 12 months after they end, by a daily job.
- **Closed accounts:** every day the Product reports the accounts it holds data about to Atlassian, and erases the account IDs of accounts Atlassian reports as closed.
- **Least privilege:** the Product requests only the Atlassian permission scopes it needs.
- **Teamvane's own access:** Teamvane has no tool to browse the data stored in the Customer's site. It can read the Product's error logs while the Customer's admins allow log sharing (Atlassian Administration → Connected apps → the Product → Logs access). Teamvane's accounts use two-step verification.
- **Testing:** automated tests check the privacy and permission rules before each release.

## Annex IV – List of sub-processors

| Sub-processor | What it does | Location |
| --- | --- | --- |
| Atlassian (Atlassian Pty Ltd and its affiliates) | Runs the Product on the Forge platform, stores its data, delivers live updates and keeps logs | The same location as the Customer's Jira site data. Atlassian's own sub-processors are listed on [atlassian.com](https://www.atlassian.com/legal/sub-processors). |
