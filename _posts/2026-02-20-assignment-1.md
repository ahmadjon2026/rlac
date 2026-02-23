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
_**Institutional Language Is Stronger in Rowling.**_ To measure institutional authority, I examined words such as *professor, ministry, headmaster, detention,* and *rules* across all six texts.

As shown in the code below, I manually defined two keyword groups in R to represent institutional authority and self-directed agency. This allowed me to systematically compare how these two types of language appear across the six texts. The frequency counts generated from these keyword lists form the basis of the visualizations that follow.

```
authority_words <- c("professor", "ministry", "headmaster", "rules", "detention")
agency_words    <- c("plan", "planned", "decide", "decided", "lead", "leading", "choose", "chose")
```
<br>
<div style="text-align: center;">
  <img src="https://ahmadjon2026.github.io/rlac/assets/images/posit_agency_authority.jpg" 
       alt="Bar graph showing frequency of authority-related words in Rowling and fanfiction texts">
  <br>
  <em>Figure 1. Authority vs Agency Words (Total Counts)</em>
</div>
<br>
*Figure 1* shows a clear difference. Authority-related words appear far more frequently in Rowling’s novels than in the fanfiction texts. The gap is substantial, not minor. This suggests that institutional vocabulary is central to Rowling’s narrative world. The school, the Ministry, and formal hierarchy are linguistically visible and repeated. In fanfiction, authority terms are present but less dominant. Institutions are not removed, but they are less saturated in the language.

To examine distribution within individual texts:

<div style="text-align: center;">
  <img src="https://ahmadjon2026.github.io/rlac/assets/images/posit_heatmap.jpg" 
       alt="Bar graph showing frequency of authority-related words in Rowling and fanfiction texts">
  <br>
  <em>Figure 2. Keyword Heatmap (Relative Frequency)</em>
</div>
<br>
The heatmap confirms that authority words cluster more strongly in Rowling’s novels. Fanfiction texts show lighter frequency patterns.

Voyant trends support this pattern.

<div style="text-align: center;">
  <iframe style="width: 544px; height: 350px;" 
          src="https://voyant-tools.org/tool/Trends/?query=headmaster*&query=ministry*&query=professor&query=dumbledore*&corpus=a6897725c6bad7a67d353cc608483d70">
  </iframe>
  <br>
  <em>Figure 3. Voyant Trends: Institutional Terms</em>
</div>
<br>
The trend lines show that words like *professor* and *dumbledore* peak in the original novels and decline in fanfiction. The decline is consistent across texts.

Overall, authority vocabulary is the clearest lexical difference between the two corpora.

## Findings Part 2:  Agency Language
_**Agency Increase Is Modest and Uneven.**_ I expected to find a strong increase in self-directed words such as *decide, plan, lead,* and *control* in fanfiction.

<div style="text-align: center;">
  <img src="https://ahmadjon2026.github.io/rlac/assets/images/posit_agency_authority.jpg" 
       alt="Bar graph showing frequency of authority-related words in Rowling and fanfiction texts">
  <br>
  <em>Figure 1 (again). Authority vs Agency Words (Total Counts)</em>
</div>
<br>
Agency terms appear slightly more often in fanfiction than in Rowling’s novels. However, the difference is limited. The increase is visible but not dramatic.
To examine variation across texts:

<div style="text-align: center; margin-bottom: 30px;">
  <iframe style="width: 544px; height: 350px;" 
          src="https://voyant-tools.org/tool/Trends/?query=plan*&query=control*&query=decide*&query=lead*&corpus=a6897725c6bad7a67d353cc608483d70">
  </iframe>
  <br>
  <em>Figure 4. Voyant Trends: Agency Terms</em>
</div>

The trend lines show uneven distribution. Some fanfiction texts show noticeable increases in words like *plan* or *lead,* while others remain close to Rowling’s baseline levels. This suggests that agency is not uniformly intensified in fanfiction. It appears concentrated in particular narratives rather than consistently elevated.

The heatmap supports this interpretation, showing variation rather than a clear structural shift. The lexical increase in agency language is therefore weaker than expected.

This complicates the assumption that fanfiction automatically produces greater character autonomy at the level of vocabulary.

## Qualitative Layer: “Must”
To move beyond frequency counts, I examined the word _**must**_ in context.

<div style="text-align: center;">
  <img src="https://ahmadjon2026.github.io/rlac/assets/images/visual4.jpg" 
       alt="Bar graph showing frequency of authority-related words in Rowling and fanfiction texts">
  <br>
  <em>Figure 5. Voyant Context: “Must” in Rowling</em>
</div>
<br>
In Rowling’s novels, *must* often appears in institutional commands. It reinforces obligation and hierarchy.

<div style="text-align: center;">
  <img src="https://ahmadjon2026.github.io/rlac/assets/images/visual5.jpg" 
       alt="Bar graph showing frequency of authority-related words in Rowling and fanfiction texts">
  <br>
  <em>Figure 6. Voyant Context: “Must” in Fanfiction</em>
</div>
<br>
In fanfiction, *must* appears in more varied contexts. It is sometimes used in negotiation, internal thought, or emotional exchange. This suggests that authority shifts not only in quantity but in tone.

## Reflection
This project started with a clear expectation. I thought fanfiction would reduce institutional language and increase language of agency. At first, the results seemed to confirm this idea. In *Figure 1,* authority-related words appear much more often in Rowling’s novels. Agency words appear slightly more in fanfiction. The difference looks strong.

However, when I looked more closely, the pattern became more complex.

The large authority gap is mainly caused by one word: “professor.” In the Voyant trends, the words “ministry” and “headmaster” remain almost stable across all six texts. The heatmap shows the same thing. The strong difference in *Figure 1* is not spread evenly across all institutional words. It is concentrated in a single word. This weakens my original claim. The high frequency may reflect the school setting itself rather than a deep structural dominance of authority.

This shows why distant reading must be handled carefully. The *High Theory* podcast explains that distant reading works at a *“macroscopic scale”* but still requires close interpretation. The total counts looked decisive. The trend lines made the picture more nuanced. The method revealed a pattern, but it also forced me to question it.

The same issue appears in the agency category. I expected a clear increase in verbs such as “decide,” “plan,” and “lead” in fanfiction. Instead, the rise is modest. The word “plan” peaks strongly in one fanfiction text, but the others remain close to Rowling’s level. “Decide” and “lead” are only slightly higher overall. The shift toward agency exists, but it is limited and uneven.

Here Underwood’s warning about the *“illusion of objectivity”* becomes important. Graphs look clear and convincing. But numbers do not interpret themselves. If I had relied only on the total bar graph, I would have overstated the difference. The method demands self-doubt.

The qualitative analysis of the word **“must”** was more revealing than the frequency counts. In Rowling, phrases like *“Harry Potter must”* appear often. Obligation is placed on the character from outside authority. In fanfiction, phrases such as *“I must”* and *“We must”* appear more frequently. Obligation becomes internal and personal. Authority does not disappear, but it shifts location.

This supports what Kestemont and Herman argue when they describe computational models as tools that reshape interpretation rather than replace it. The data did not prove that fanfiction rejects institutions. Instead, it showed a subtle redistribution of authority from formal titles toward internal voice.

In the end, the strongest lexical difference is the repetition of **“professor”** in Rowling. The increase in agency language is present but modest. This forces a more careful conclusion. Fanfiction does not radically dismantle institutional language at the level of vocabulary. It slightly softens it and shifts its tone.

Distant reading did not dramatically confirm my hypothesis. Instead, it *corrected* it. **That correction is the most valuable outcome of this project.**



**"READY FOR GRADING"** - I think so 🤔