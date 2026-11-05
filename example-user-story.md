---
title: Example User Story
summary: A worked example of how a single missing API data field became a user story, a Given/When/Then, and three test cases.
role: Product Owner
period: 2021 – 2023
tags: [user-story, acceptance-criteria, apis, test-cases, agile]
---

# Example User Story

- **Role** — Product Owner
- **Stakeholders** — Internal stakeholders (teams using the search APIs)
- **Team** — Public Site Search

**Overview:** The search servlets were migrated to ECS and then to Lambda. The most requested, number-one frustration our internal partners had was the sort order of the data from the APIs. It was critical to their release priority to get this fixed before they went live to their users.

## 1. The Problem

The data delivered via the API had no added field that would allow the internal teams to sort the data displayed in their applications. This caused quite a headache, because a query for *Apple* yielded a bunch of stocks and ETFs with the word "apple" in their names — but not the actual company Apple Inc., which is what the vast majority of people are looking for when they type in the word *apple*.

## 2. The User Story

> As a developer using the search APIs, I need another data field that will allow me to sort the names of stocks, ETFs, and mutual funds, so that when one of my customers searches a major corporation (e.g. Apple, IBM, Nvidia), that major corporation shows at the top of the search box's drop-down suggestion list.

## 3. GWT

> **Given** that a user will type *keywords* in the search box  
> **When** they want to find a particular stock, ETF, or mutual fund  
> **Then** the most recognizable stock, ETF, or mutual fund associated with their search term should appear at the top  
> **So That** they can buy, sell, or exchange the stock, ETF, or mutual fund quickly and easily.

## 4. The Recommendation

Add an additional data point to the API that will allow the developers using the APIs to sort the data displayed in their search box's drop-down suggestions.

The recommended data point is the previous day's end-of-trade volume.

## 5. The Test Cases

**Test Case 1 — keyword search**  
Type the word *apple* into the trade lab's search box.  
*Expected result:* AAPL (Apple Inc.) shows at the top of the drop-down suggestion box.

**Test Case 2 — keyword search**  
Type the word *IBM* into the trade lab's search box.  
*Expected result:* IBM (IBM Inc.) shows at the top of the drop-down suggestion box.

**Test Case 3 — stock symbol search** *(repeat with ETF and mutual fund ticker symbols)*  
Type *NVDA* into the search box.  
*Expected result:* NVDA should be the **first** stock showing in the drop-down.

<!-- nav -->
[← Cross-Site Comparison](cross-site-comparison.md)  ·  [All case studies](/)  ·  [Too Many Clicks →](too-many-clicks.md)
