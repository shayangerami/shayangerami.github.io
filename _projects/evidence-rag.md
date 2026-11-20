---
layout: page
title: EvidenceEval
description: Evidence-aware RAG agent and evaluation framework
img: # optional card image, e.g. assets/img/projects/evidence-rag.jpg
importance: 1
category: independent
github: https://github.com/shayangerami/EvidenceEvalRAG
---

**EvidenceEval: Evidence-Aware RAG Agent and Evaluation Framework**

A retrieval-augmented generation agent that checks whether retrieved evidence supports its answer before responding, and abstains when it does not.

#### Highlights

- Built a LangGraph agent with local Qwen2.5 models, semantic retrieval, evidence verification, a hybrid retrieval retry, and abstention.
- Across 300 SciFact claims, the automated unsupported-answer rate fell from 37.7% for the semantic RAG baseline to 7.3% with the agent.
- The framework also tracks answer coverage and latency. The agent abstained on 58.0% of answerable claims versus 28.7% for the baseline, so the gain in reliability comes with lower coverage.

Code: [github.com/shayangerami/EvidenceEvalRAG](https://github.com/shayangerami/EvidenceEvalRAG)
