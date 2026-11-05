---
title: Advanced Search
summary: Regex analysis of a million queries found Boolean operators in use by a small but real niche — then usability testing showed the proposed tool was not worth prioritizing.
role: Product Owner
period: 2016 – 2019
tags: [search, boolean-operators, regex, usability-testing, prototyping, prioritization]
---

# Advanced Search

- **Role** — Product Owner
- **Stakeholders** — Business units (Digital), senior directors (Digital Commerce)
- **Team** — Cross-collaborative

**Overview:** The single search box has become the ubiquitous standard for all search boxes, regardless of the context of their existence. They are also accompanied by the expectation that they will function like Google. But our data is not indexed in the same way that Google's is.

## 1. The Problem

Using the single search box gives the impression that our search will function like the search giant Google. It does not. We found numerous instances in the query data that showed uses of conditional, or Boolean, operators in a Google-like attempt to define queries with specificity. The back-end search code is not set up for this type of search query.

## 2. The Hypothesis

Providing a method for these mission-oriented searchers would improve their search experience while decreasing the time they spend using navigational filters to narrow their results set. Creating an "advanced search" option would allow them to target specific data fields.

## 3. The Goals

The primary objective is to provide a tool for precise search. The secondary objective is to improve the efficiency of the searching. The measures for these objectives:

- reduction in repetitive searching (defined as one search followed by a second search in less than 10 seconds)
- increase in "add to list" and/or "add to cart" from the search results page
- decrease in negative VOC feedback

## 4. The Quantitative Data

The top 1 million search queries were extracted from Adobe Analytics for a 90-day period. Using regular expressions, the following conditional, or Boolean, operators were found:

```
AND   OR   NOT   -   +   " "   /   %   ' '
```

While the overall percentage of use is below 5% of total users, it is enough of a niche group of customers for us not to ignore.

## 5. The Usability Test Scenarios

![Current single search box alongside the advanced search prototype, which offers AND, OR, NOT, and IN rows plus category, family, and attribute selectors](images/advanced-search-wireframe.png)

For each participant of the usability test, the tester will show them the search box and the advanced search feature prototype. The tester will emphasize the need for the advanced search feature's use during the test.

> **Scenario 1** — You are in the first round of prototyping a new printer connector. Your goal is to make the connector smaller, which means you need a tighter configuration of pins, or fewer pins altogether. How will you find this part?

> **Scenario 2** — You have a part number, but upon looking it up you discover that the part has been upgraded. The new specifications do not meet the needs for your project. Find an alternative.

> **Scenario 3** — You have always referred to the part in your hand as a micro connector, but when you do this search, the results look nothing like the thing you are holding. Using other descriptive features, find the part on the website.

## 6. Findings & Recommendation

Out of the 8 participants, only 3 were comfortable using the advanced search feature. The 3 who used it found it useful, but noted that some parts they expected to see were missing — most likely due to incomplete data.

While the tool would help some of our customers, the majority would overlook it as unnecessary. Therefore, we do not consider this a high-priority need at this time.

<!-- nav -->
[← Type Ahead Redesign](type-ahead-redesign.md)  ·  [All case studies](/)  ·  [Country Selector →](country-selector.md)
