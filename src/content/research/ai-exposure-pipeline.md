---
title: "Estimating AI Automation Exposure for 60,000 Occupational Records"
type: "Research project (ongoing)"
role: "Researcher"
date: 2026-10-01
dateLabel: "May 2026 – ongoing"
venue: "Korea Information Society Development Institute (KISDI)"
location: "Jincheon"
collaborators:
  - "Dr. Aram Moon (supervisor)"
cover: ./ai-exposure-pipeline/cover.png
coverCaption: "Within-job variance of automation-exposure scores by model (log scale): Claude is the most consistent across repeated runs, ChatGPT the least."
summary: "A retrieval-augmented LLM pipeline that estimates AI automation potential for 60,000 occupational records, cutting an estimated month of manual labeling to two days."
featured: true
---

This work was part of the KISDI project "AI Transition and Global Structural Change." The question was how to estimate the potential for AI automation across a very large set of occupational records without labeling each one by hand.

I developed an LLM pipeline with retrieval-augmented generation (RAG) to score 60,000 occupational records. It used ILO ISCO-08 exposure estimates (Gmyrek et al., 2025) as reference data, and each record was scored with reference to its most similar occupations. Occupational similarity and score similarity were strongly correlated (r = 0.88).

The pipeline cut a labeling task expected to take about a month down to two days. I also maintained the structured dataset of AI exposure estimates and carried out statistical analyses of how exposure varies across occupations. The work was supervised by Dr. Aram Moon.

The project is ongoing. One line of work compares how consistently different language models score the same job across repeated runs, and how their score distributions differ.

![Distribution of automation-exposure scores by model: ChatGPT (mean 0.320), Claude (0.287) and Gemini (0.352).](./ai-exposure-pipeline/fig-1.png)
