---
title: Cross-Site Search Comparison
summary: Manually tagging 42,765 queries across four properties to test — and largely disprove — the belief that irrelevant search results were caused by customers landing on the wrong site.
role: Product Owner
period: 2022
tags: [query-analysis, controlled-vocabulary, manual-tagging, search, data-analysis]
---

# Cross-Site Search Comparison

- **Role** — Product Owner
- **Stakeholders** — Product owners for search on other properties
- **Team** — Individual analysis

**Overview:** A common belief permeated the various marketing teams — that a large number of searches on the various properties actually should have occurred on a different property, and that this was causing the complaints about irrelevant searches. In other words: the customer was lost; the content was fine.

## 1. The Method

Manual tagging of at least 10% of the queries from each dataset was applied.

Because the dataset from the Personal Investor site was the largest, its topic set was used as the controlled vocabulary for all four datasets.

Excel formulas were used to determine:

- number of characters per query
- number of words per query

## 2. The Data

Datasets from the four major US properties were obtained:

- `corporate.vanguard.com` (Corporate)
- `ownyourfuture.vanguard.com` (Institutional)
- `investor.vanguard.com` (Personal Investor)
- `advisors.vanguard.com` (Financial Advisory)

Each dataset contained queries from the same timeframe, March to May 2022.

| Site | Queries submitted | Queries analyzed | Percentage |
|---|---:|---:|---:|
| Personal Investor | 50,000 | 36,462 | 73% |
| Corporate | 9,112 | 4,367 | 48% |
| Financial Advisory | 7,583 | 790 | 10% |
| Institutional | 5,415 | 1,146 | 22% |
| **Totals** | **72,110** | **42,765** | **59%** |

## 3. The Findings

| | Personal Investor | Corporate | Financial Advisory | Institutional |
|---|---|---|---|---|
| **Avg. characters / query** | 15.8 | 17.7 | 3.6 | 22.1 |
| **Avg. words / query** | 2.6 | 2.9 | 1 | 3.3 |
| **Most searched** | *rmd* — 11,987 | *login* — 1,096 | *vti* — 1,017 | *voo* — 398 |
| **Fewest searched** | *4* — 3 | *x*, *n*, *wh*, etc. — 1 | *vfwpx*, *540*, etc. — 1 | *s* — 1 |
| **Shortest queries** | 37 single-character queries, 26 were stocks | 10 single-character queries, 9 were stocks | 24 single-character queries, 23 were stocks | 2 single-character queries, 1 was a stock |
| **Longest query** | 50 words, 255 characters | 63 words, 320 characters | 18 words, 120 characters | 16 words, 91 characters |

![Full findings comparison across the four properties](images/findings-comparison-table.png)

### Major topics by site

- **Personal Investor** — transfer, fund, stock, form, account, tax, rmd, withdraw, statement, change, beneficiary, rollover deposit, contact, buy, watchlist, open, close, qcd, sell
- **Corporate** — account, fund, Vanguard, keyword, etf, products, transact, form, tax, help, strategy, stock corporation, industry, advice, bond, shareholders, performance
- **Financial Advisory** — ETF Share Class, Admiral Share Class, Investor Share Class, keyword, fund, stock, Institutional Share Class, Institutional Plus Share Class
- **Institutional** — Admiral Share Class, ETF Share Class, keyword, Institutional Share Class, fund, total, Investor Share Class, Institutional Plus Share Class, target, Form, bond, account

## 4. Cross-over

![Nested circles showing query cross-over: 92% Financial Advisory, 85% Institutional, 79% Corporate, all nested inside Personal Investor](images/query-crossover-venn.png)

1. All queries from Corporate, Institutional, and Financial Advisory would yield a search result of some kind on Personal Investor.
2. Most queries from Personal Investor, Financial Advisory, and Institutional would, for the most part, work interchangeably among the three sites, due to a high volume of searches for funds, ETFs, and securities.
3. Nearly all queries from Financial Advisory and Institutional would **not** yield results on Corporate, due to the high volume of fund, ETF, and security queries.
4. Some Financial Advisory and Corporate queries are interchangeable.
5. Nearly 80% of the queries on Corporate would work on Personal Investor, Financial Advisory, and Institutional — and would yield better results on those three sites than on Corporate.

<!-- nav -->
[← Migration to New Search](migration-to-search.md)  ·  [All case studies](/)  ·  [Example User Story →](example-user-story.md)
