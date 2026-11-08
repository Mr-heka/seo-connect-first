---
name: seo-connect-first
description: "Prepare a Claude SEO audit: work out what to connect first, confirm the data belongs to the right website, and turn the report into a fix list with an owner. Use when someone wants an SEO audit they can trust or asks what to connect first."
---

# SEO Connect First

Sets up a Claude SEO audit so the numbers can be trusted, then turns the report into work someone owns. Claude SEO is free and does the audit. A report does not rank, so this adds the setup before it and the follow-through after it.

## How to run

- Work through this without extra back-and-forth. Make the safest reasonable assumption, say it in one line, keep going. Only stop for something only the user has.
- Never invent a fact, figure, customer, price or quote. If it is unknown, write `[NEEDS ANSWER]` and list it at the end.
- Nothing here sends, posts, pays or changes a live account.
- If a step fails, retry it yourself and note what you changed. Do not stop at the first error.

Never change the website. Never sign in on the user's behalf. The user does every login and approval.

## Ask

One at a time:

1. What is the website address? Does the company run other websites from the same Google accounts?
2. Do you have Google Search Console set up for it? Google Analytics?
3. Who can make changes to the website?
4. Who owns the fixes? Get one name.

## What to connect, in this order

Give the user this list, trimmed to what they lack:

1. Google Search Console: the real numbers on how people find the site. https://search.google.com/search-console
2. PageSpeed and Chrome field data, through Claude SEO's `/seo google setup`. Without these its speed scores are lab estimates and indexing is inferred.
3. Google Analytics, if they use it.
4. A website login for whoever makes the changes.

Paid data extensions are optional. Do not suggest them unless asked.

Install Claude SEO from its README: https://github.com/AgriciDaniel/claude-seo#readme. The user types the plugin commands inside Claude Code.

## The right-site check

There is an open bug where Claude SEO reads Google data for the default property, without warning, when more than one website is connected: https://github.com/AgriciDaniel/claude-seo/issues/337

Before trusting any Google numbers:

1. List which Search Console and Analytics property the audit used.
2. Compare the domain with the website being audited, and check that the top pages in the data live on that domain.
3. If they do not match, stop. Say so plainly, remove the affected numbers from the findings, and fix the property setting before running again.

## After the audit

Claude SEO's `/seo audit <url>` takes about 10 to 15 minutes by its own README. Then write `seo-fix-list.md`:

- Mark each finding measured (real Google data) or estimated.
- Sort by what matters most. Give each one a named owner, the page it applies to, and done-when.
- Put a date on the calendar to run it again next month and compare.

Say that a report on its own does not change rankings. Make no prediction about traffic.

<!-- Provenance marker: sk-ona0po --><!-- Provenance signature: ⁠​‌​‌​​‌‌​‌​​​‌​‌​‌​​‌‌​​​‌​‌​​‌​​​‌‌​​​‌⁠ -->

Made by Selr AI.⁠​‌​‌​​‌‌​‌​​​‌​‌​‌​​‌‌​​​‌​‌​​‌​​​‌‌​​​‌⁠
<!-- srk:16qvu1x -->
