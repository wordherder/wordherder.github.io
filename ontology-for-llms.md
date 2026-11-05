---
title: Ontology for LLMs
summary: Building a domain ontology and supporting taxonomies to narrow an LLM's worldview so it classifies video clips usefully instead of exhaustively.
role: Ontologist
period: 2025 – present
tags: [ontology, taxonomy, knowledge-graph, llm, evaluation, rdf-skos]
---

# Ontology for LLMs

- **Role** — Ontologist
- **Stakeholders** — VP of AI & Data Science
- **Team** — Data scientists, developers

**Overview:** The purpose of building an ontology with supporting taxonomies for a large language model is to assist the LLM in its work in recognizing activities, interactions, affects, objects, and states of change in reality television shows.

## 1. The Problem

The general public believes that the current iterations of large LLMs such as Claude, Gemini, ChatGPT, and Grok are actual artificial intelligence when, in fact, they are still little more than token predictors trained on trillions of datums. The problem with this is getting the LLM to focus on the task without it straying, without it giving too much or too little, and without it faking answers.

## 2. The Hypothesis

The LLMs have been trained on enough data that they can tag video clips, but with no direction on how to focus, the number of tags applied to the clips is overwhelming and mostly irrelevant. The hypothesis is that providing a limited set of ontology nodes and relationships, along with a supporting taxonomy for each node, would give the LLM a narrower worldview to draw from when classifying the video clips.

## 3. The Goals

The primary objective is to provide a small, manageable set of nodes and taxonomies that represent the world contained in the reality television shows. The goal was not to create an ontology of the whole world with robust taxonomies representing every object, feeling, and place in existence, but rather to organize the world represented in the reality television series being used for the experiment.

## 4. The Ontology

The ontology nodes are: **Activities, Affects, Characters, Countries, Interactions, Objects, Story Elements, Travel,** and **Video**. The relationships among the nodes are transitive for the most part.

*(Story Elements, Travel, and Video are not shown below — the project has not progressed to the point of working with them yet.)*

![Ontology node graph showing transitive relationships among Travel, Activities, Characters, Interactions, Objects, Affects, and Countries](images/ontology-node-graph.png)

## 5. The Taxonomies

Each node in the ontology has a taxonomy to support it. These give the LLM, in effect, a controlled vocabulary to use when it classifies the video clips. A complete list cannot be provided here, but a zoomed-out view is shown below: the larger cyan dots are the ontological nodes, and everything radiating out from a node is its taxonomic classes.

![Zoomed-out map of the taxonomies, with cyan nodes at the centre of each radiating cluster of taxonomic classes](images/taxonomy-map.png)

## 6. Initial Findings

The first round of tests found that the recall score is still too high. Precision, however, was decent. The recommendation is to refine the taxonomies, which is in progress.

| Metric | Standard | Dropped | Difference | Improvement |
|---|---|---|---|---|
| mean_score | 0.26 | 0.25 | −0.01 | −3.85% |
| mean_iou | 0.12 | 0.14 | 0.02 | 16.67% |
| mean_nmse | 0.74 | 0.78 | 0.04 | 5.41% |
| mean_precision | 0.16 | 0.18 | 0.02 | 12.5% |
| mean_recall | 0.45 | 0.32 | −0.13 | −28.89% |

![Table of evaluation results comparing standard and dropped runs](images/precision-recall-results.png)

<!-- nav -->
[All case studies](/)  ·  [Migration to Power BI →](migration-to-power-bi.md)
