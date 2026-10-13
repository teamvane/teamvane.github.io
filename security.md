---
title: Security – Teamvane
permalink: /security/
---

<!--
DRAFT for review. Fill [DATE] with the publication date before publishing.
Needs the security@teamvane.com alias to exist.
-->

# Security

**Last updated:** [DATE]

This page explains how Teamvane, the trading name of Alexandre Blasco Brasó, based in France, builds and looks after its apps for Atlassian products, and how to report a security problem.

## Reporting a vulnerability

Email **security@teamvane.com** with:

- the app and, if you know it, the version;
- what you found and how to reproduce it;
- what an attacker could do with it.

We will acknowledge your report within **two business days**, keep you informed, and tell you when it is fixed. Please give us a reasonable time to fix a problem before you disclose it publicly. We will not take legal action against anyone who reports a vulnerability in good faith, avoids harming our customers and their data, and doesn't access more data than needed to show the problem.

Atlassian also runs a [Vulnerability Disclosure Program](https://developer.atlassian.com/platform/marketplace/vdp/) for Marketplace apps.

## How quickly we fix vulnerabilities

We follow Atlassian's [Security Bug Fix Policy for Marketplace apps](https://developer.atlassian.com/platform/marketplace/security-bugfix-policy/). For cloud apps, counted from when a vulnerability is reported or triaged:

| Severity (CVSS) | Fixed within |
| --- | --- |
| Critical (9.0 and above) | 10 days |
| High (7.0 to 8.9) | 4 weeks |
| Medium (4.0 to 6.9) | 12 weeks |
| Low (below 4.0) | 25 weeks |

Fixes reach every customer through Atlassian's automatic app updates.

## How our apps are built

- **Runs on Atlassian.** Our apps are built on Atlassian Forge and run entirely on Atlassian's infrastructure. We have no servers or databases of our own, and our apps send no data outside Atlassian.
- **Least privilege.** Each app requests only the Atlassian permissions it needs, and acts with the signed-in user's own permissions whenever it reads or changes data in Jira.
- **Checks on the server.** Permission and business rules are enforced on the server, never only in the browser.
- **Data minimisation.** Our apps store as little personal data as they can, delete it automatically when it's no longer needed, and erase the data of closed Atlassian accounts as Atlassian requires.
- **No access to customer data.** We have no tool to browse the data our apps store in customer sites. We can read error logs only while a customer's admins allow log sharing.
- **Testing.** Automated tests check each app's security and privacy rules before every release.
- **Dependencies.** We keep dependencies to a minimum and update them when security fixes are released.
- **Accounts.** The accounts we use to build, publish and support our apps are protected with two-step verification.

## Security incidents

If an incident affects a customer's data, we will notify that customer without undue delay, and where possible within 48 hours of becoming aware of it, as set out in each app's Data Processing Addendum. We also follow Atlassian's [Partner Security Incident Response Program](https://developer.atlassian.com/platform/marketplace/partner-security-incident-response-program/).

## Contact

Security problems: **security@teamvane.com**. Everything else: **support@teamvane.com**.
