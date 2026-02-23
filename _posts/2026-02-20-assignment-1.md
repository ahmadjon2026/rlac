---
title: "Assignment 1"
categories:
  - assignments

---

## Introduction
J.K. Rowling’s early Harry Potter novels are structured around institutions. Hogwarts, the Ministry of Magic, school rules, professors, and formal hierarchies shape the world of the story. Authority is visible and organized. Power often flows through official positions such as headmaster, professor, or ministry official. Even when characters resist authority, they do so within a clearly defined institutional framework.

Fanfiction rewrites and expands this world. Many readers and writers see fanfiction as a space of greater freedom. It allows characters to act differently, question authority, or reshape relationships. A common assumption is that fanfiction shifts the focus away from institutions and toward personal choice and self-direction.
 
This project asks whether that shift appears at the level of language. Does fanfiction reduce institutional vocabulary and increase words that signal agency and self-directed action? I expected to find a strong decrease in authority language and a clear increase in verbs associated with choice and control in fanfiction texts. To test this expectation, I use distant reading tools to compare selected early novels by Rowling with several fanfiction works set in the same universe.

## Method
This project compares three early Harry Potter novels by J.K. Rowling: *Harry Potter and the Sorcerer’s Stone,* *Harry Potter and the Chamber of Secrets,* and *Harry Potter and the Prisoner of Azkaban.* These novels establish the institutional structure of the wizarding world and form the canonical baseline for this analysis.

They are compared with three fanfiction texts set in the same universe: *Resurrection* by Sugahhuney, *HP Next Gen* by toomanyfandoms, and *Reconstructing HP* by yellowsunchild. These works were selected because they reimagine the Harry Potter world while retaining its central characters and setting.

The texts were analyzed using Voyant Tools and R with the tidytext package. In both platforms, the corpus was cleaned by removing common stopwords. In the R analysis, character names were also removed to prevent them from dominating frequency counts and visualizations.

Two lexical categories were constructed for comparison. The first category represents institutional authority and includes words such as **professor, ministry, headmaster, detention,** and **rules.** The second category represents agency and self-direction and includes verbs such as **decide, choose, plan, lead,** and **control.** These word lists were selected based on their relevance to the research question and were applied consistently across all texts.

The analysis included word frequency counts, trend graphs, contextual views, a heatmap, and word clouds. These visualizations were used to identify differences in distribution and intensity between the Rowling texts and the fanfiction texts. Because the corpus is relatively small, the results indicate tendencies rather than universal conclusions.

## Findings Part 1: Authority Language
_**Institutional Language Is Stronger in Rowling.**_ To measure institutional authority, I examined words such as professor, ministry, headmaster, detention, and rules across all six texts.

<div align="center">
  <img src="/assets/images/posit_agency_authority.png">
  <br>
  <em>Figure 1. Frequency of Institutional Language</em>
</div>

