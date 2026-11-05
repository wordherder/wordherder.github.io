---
title: Migration to Power BI
summary: Standing up a brand-new team and moving hundreds of reports off Qlik Sense before the contract expired, while training that team in Agile at the same time.
role: Product Owner
period: 2024 – 2025
tags: [migration, power-bi, agile, dbt, aws, stakeholder-management]
---

# Migration to Power BI

- **Role** — Product Owner
- **Stakeholders** — Employees (company-wide)
- **Team** — Cross-collaborative

**Overview:** The company had decided to pivot to Power BI as the enterprise standard for the analytics reporting platform. As a result, it decided not to renew the contract for the old platform, Qlik Sense. The contract expires on July 31, 2025. All reports must be moved to Power BI to ensure productivity does not drop.

## 1. The Problem

Qlik Sense as a platform for analytics reporting is antiquated. It has no artificial intelligence capabilities and, worse, its data load time is extremely slow. While its workhorse ways get the job done and employees are comfortable with its rhythms, it is actually wasting a great deal of time and costing the company money. Nearly every day, reports are broken and do not load current data, and this leads to misinformed decision-making across the business.

## 2. The Need

Employees need accurate and timely data in order to make the best decisions for the company. Without that capability, employees are unable to move swiftly when opportunity presents itself. The "fear of missing out" becomes a reality rather than an abstract anxiety, and the company loses real money — which the shareholders, of course, do not like.

## 3. The Objective

The goal placed before the newly formed team is to migrate the hundreds of reports out of Qlik Sense over to Power BI by the July 31, 2025 deadline. The team was formed in June 2024 and fully staffed by October 2024.

1. Train the new team in Agile methodology.
2. Migrate the reports (pursued concurrently with objective 1).
3. Optimize the reports so that there are fewer but better ones.

## 4. The Plan

The first report suite had been partially migrated already, in a haphazard fashion. The plan was to have the consulting company complete that migration and train the new team in the process. Following that, the remaining report suites would be migrated by the new team alone, without the assistance of a consulting firm.

## 5. Timeline

![Project timeline running from June 2024 hiring through July 2025 break/fix, with report suites delivered monthly from December 2024 onward](images/powerbi-timeline.png)

- **June 2024** — Hired; Agile training, Qlik research
- **July 2024** — Power BI training
- **August 2024** — Onboarding consultants
- **September 2024** — Requirements gathering
- **October 2024** — AWS requirements, DBT development
- **November 2024** — UX design, Power BI build
- **December 2024** — Release of 1st report suite
- **January 2025** — 3 report suites
- **February 2025** — 2 report suites
- **March 2025** — 4 report suites
- **April 2025** — 3 report suites
- **May 2025** — 3 report suites
- **June 2025** — 3 report suites
- **July 2025** — Break/fix

## 6. The Process

![Process flow: surveys/workshops, data lineage and KPI tree feed wireframes; BUS ERP feeds AWS; wireframes and AWS feed DBT, then Power BI build, data validation, and launch](images/powerbi-process-flow.png)

Surveys/workshops, data lineage, and a KPI tree feed the wireframes. In parallel, BUS ERP data lands in AWS. Wireframes and AWS data feed DBT, which feeds the Power BI build, then data validation, then launch.

## 7. Project Learnings So Far

Working with a consulting agency may have cost the new team too much time. It may have been better to work with the initial group of people who had started the first report suite migration on their own, however haphazard it had been at the time. What the consulting agency achieved over four months was achieved by the "unofficial" team in a week. The amount of time the consulting agency took to ramp up and then actually do the project was underwhelming, and remarkably stifling to the new team created for the migration.

Due to the setback, the newly formed team is having to speed up the report suites' migration timeline by doing a lift-and-shift and cutting back the optimization piece of the project.

<!-- nav -->
[← Ontology for LLMs](ontology-for-llms.md)  ·  [All case studies](/)  ·  [Migration to New Search →](migration-to-new-search.md)
