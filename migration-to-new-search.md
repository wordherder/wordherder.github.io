---
title: Migration to New Search
summary: Three concurrent platform migrations on a single decade-old search page, taking onsite search traffic from under 1% to 5% and zero-result searches from 12% to 0.68%.
role: Product Owner
period: 2021 – 2022
tags: [search, coveo, aem, medallia, migration, relevancy-tuning, voc]
---

# Migration to New Search

- **Role** — Product Owner
- **Stakeholders** — Clients, prospects, employees
- **Team** — Cross-collaborative

**Overview:** The Personal Investor search page had not been touched in a decade. The search engine was equally antiquated. Even the feedback survey on the page was still using an outdated platform. This one page required three migrations: OpinionLab to Medallia, Teamsite to AEM, and Autonomy to Coveo.

## 1. The Problem

Less than 1% of the onsite traffic bothered to use the search function on the website. Those who did use it were greeted with highly irrelevant results, or with no results at all — nearly 12% of searches yielded zero results. The feedback survey on the search results page averaged 600 responses per month, all complaints about search's inability to provide useful results.

## 2. The Need

Clients and prospects needed a reliable search tool that would help them find answers to their questions quickly and efficiently when the browse navigation failed to guide them. Client support also needed a search tool that provided good results so that clients could self-serve and thereby reduce call volume.

## 3. The Objective

1. Replace the ancient search engine Autonomy with the modern machine-learning platform Coveo.
2. Update the look and feel of the page by building a new page in Adobe Experience Manager, as part of the broader website modernization initiative.
3. Update the search page's feedback survey to the modern survey platform Medallia, with a simpler, easier set of questions to answer.

## 4. The Plan

Objectives 1 and 2 were prioritized as most important. Objective 3 was decided to be a "nice to have" if it could be done in the timeline proposed. While it was never a date with a hard stop, the tech leads and architects agreed that objectives 1 and 2 could be completed within a year, as the migration of each platform could occur concurrently.

## 5. Timeline

![Timeline from June 2021 hiring through October 2022, covering UX research, prototyping, Coveo and AEM integration, phased rollout, and the new Medallia survey](images/search-migration-timeline.png)

- **June 2021** — Hired
- **June – September 2021** — UX research, workshops
- **July – September 2021** — Dev training; UX design prototype completed
- **November 2021** — First prototype in AEM completed
- **November 2021 – January 2022** — Usability testing, design updates
- **February 2022** — Coveo and AEM integration completed
- **February – July 2022** — Coveo relevancy testing and tuning
- **March 2022** — 30% rollout of new search experience
- **July 2022** — 100% rollout; objectives 1 and 2 achieved
- **October 2022** — New Medallia survey launched; all three objectives achieved

## 6. Project Learnings

Promises are not always fulfilled. The original initiative was to have the website's search experience team functioning fully independently, meaning it would have access to all three platforms: AEM, Medallia, and Coveo. Unfortunately, despite being fully trained, the search experience team's developers were not permitted access to Coveo by the marketing technology department, which created a wrinkle that nearly derailed the whole project.

A compromise was achieved by creating a component in Adobe Experience Manager that allowed the search experience team to manage the features Coveo offered — AutoSuggest labeling and how many suggestions to show, facet names and whether to show them, turning Smart Snippets on or off, and so on. But the marketing technology department retained control of the full administrative console, and all relevancy tuning requests had to go through its workflow. This, we learned, was not sustainable: that department was responsible for every website globally. A request was made to Coveo to resolve the issue, where the administrative console showed every single website's instance rather than offering a portal in which one team could be given permission to a single website instance. Coveo has yet to decide how to handle this situation.

## 7. Did the migration work?

| Measure | Result |
|---|---|
| Onsite search traffic | **< 1% → 5%** |
| No-results searches | **12% → 0.68%** |
| Click-through rate to content | **54%** |
| Decline in negative feedback | **87%** |

<!-- nav -->
[← Migration to Power BI](migration-to-power-bi.md)  ·  [All case studies](/)  ·  [Cross-Site Search Comparison →](cross-site-search-comparison.md)
