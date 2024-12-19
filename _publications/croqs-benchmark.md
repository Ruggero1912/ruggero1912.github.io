---
layout: post
title: "Maybe you are looking for CroQS 🐊 Cross-modal Query Suggestion for Text-to-Image Retrieval"
tags: query suggestion, cross-modal retrieval, text-to-image retrieval
categories: Information Retrieval, Research
author: G. Pacini et al.
published_at: European Conference on Information Retrieval 2025
image: /assets/images/publications/croqs.webp
website: https://paciosoft.com/CroQS-benchmark/
date: 2024-12-18
---

Query suggestion, a technique widely adopted in information retrieval, enhances system interactivity and the browsing experience of document collections. In cross-modal retrieval, many works have focused on retrieving relevant items from natural language queries, while few have explored query suggestion solutions.

In this work, we address query suggestion in cross-modal retrieval, introducing a novel task that focuses on suggesting minimal textual modifications needed to explore visually consistent subsets of the collection, following the premise of “Maybe you are looking for”. To facilitate the evaluation and development of methods, we present a comprehensive benchmark named CroQS. This dataset comprises initial queries, grouped result sets, and human-defined suggested queries for each group. We establish dedicated metrics to rigorously evaluate the performance of various methods on this task, measuring representativeness, cluster specificity, and similarity of the suggested queries to the original ones. Baseline methods from related fields, such as image captioning and content summarization, are adapted for this task to provide reference performance scores.

Although rather far from human performance, our experiments reveal that both LLM-based and captioning-based methods achieve competitive results on CroQS, improving the recall on cluster specificity by more than 122% and representativeness mAP by more than 23% with respect to the initial query.