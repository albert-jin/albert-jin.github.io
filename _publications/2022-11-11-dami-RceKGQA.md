---
title: "Improving embedded knowledge graph multi-hop question answering by introducing relational chain reasoning"
collection: publications
permalink: /publication/2022-11-11-dami-RceKGQA
excerpt: 'This paper is about Knowledge Graph Question Answering (KGQA).'
date: 2022-11-11
venue: 'Data Mining and Knowledge Discovery (dami)'
paperurl: 'https://doi.org/10.1007/s10618-022-00891-8'
citation: 'Biao Zhao and Weiqiang Jin et al. (2023). &quot;Improving embedded knowledge graph multi-hop question answering by introducing relational chain reasoning.&quot; <i>Data Min Knowl Disc</i>. 37, 255–288.'
---

Knowledge Graph Question Answering (KGQA) aims to answer user-questions from a knowledge graph (KG) by identifying the reasoning relations between topic entity and answer. As a complex branch task of KGQA, multi-hop KGQA requires reasoning over the multi-hop relational chain preserved in KG to arrive at the right answer. Despite recent successes, the existing works on answering multi-hop complex questions still face the following challenges: (i) The absence of an explicit relational chain order reflected in user-question stems from a misunderstanding of a user’s intentions. (ii) Incorrectly capturing relational types on weak supervision of which dataset lacks intermediate reasoning chain annotations due to expensive labeling cost. (iii) Failing to consider implicit relations between the topic entity and the answer implied in structured KG because of limited neighborhoods size constraint in subgraph retrieval-based algorithms. To address these issues in multi-hop KGQA, we propose a novel model herein, namely Relational Chain based Embedded KGQA (Rce-KGQA), which simultaneously utilizes the explicit relational chain revealed in natural language question and the implicit relational chain stored in structured KG. Our extensive empirical study on three open-domain benchmarks proves that our method significantly outperforms the state-of-the-art counterparts like GraftNet, PullNet and EmbedKGQA. Comprehensive ablation experiments also verify the effectiveness of our method on the multi-hop KGQA task. We have made our model’s source code available at github: https://github.com/albert-jin/Rce-KGQA.

Additional Key Words and Phrases: Data Mining and Search, Question Answering, Knowledge Graph based Multi-hop QA, Neural Semantic Parsing, Knowledge Graph Embedding.
