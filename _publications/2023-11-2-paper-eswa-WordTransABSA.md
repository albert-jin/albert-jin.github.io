---
title: "WordTransABSA: Enhancing Aspect-based Sentiment Analysis with masked language modeling for affective token prediction"
collection: publications
permalink: /publication/2023-11-2-paper-eswa-WordTransABSA
excerpt: 'This paper is about Aspect-based Sentiment Analysis (ABSA).'
date: 2023-11-2
venue: 'Expert Systems with Applications'
paperurl: 'https://doi.org/10.1016/j.eswa.2023.122289'
citation: 'Weiqiang Jin et al. (2023). &quot;WordTransABSA: Enhancing Aspect-based Sentiment Analysis with masked language modeling for affective token prediction,&quot; <i>Expert Systems with Applications</i>. Volume 238, Part F, 2024, 122289, ISSN 0957-4174.'
---

In recent years, Aspect-based Sentiment Analysis (ABSA) has been a crucial yet challenging task in recognizing textual emotions from text. ABSA has numerous application across various fields, such as social media, commodity review, and movie comment, making it an attractive area of research. Many researchers are working to develop more powerful sentiment analysis models. Currently, most existing ABSA models use the generic pre-trained language models (PLMs) based fine-tuning paradigm, which only utilizes the encoder parameters while discarding the decoder parameters of PLMs. However, this approach fails to leverage the prior knowledge revealed in PLMs effectively. To address these issues, we investigate the potential of the initial pre-training scheme of PLMs to conduct ABSA and thus propose a novel approach in this paper, namely Target Word Transferred ABSA (WordTransABSA). In WordTransABSA, we propose “Word Transferred LM”, a novel sequence-level optimization strategy that transferred target words in sentence into pivot tokens to stimulate better PLM semantic understanding capability. Given a sentence with aspect terms as input, WordTransABSA generates contextually appropriate semantics and predicts the affective tokens on the corresponding positions of the aspect terms. The final sentiment polarity of each aspect term is determined through several sentiment identification strategies that we selected. WordTransABSA takes full advantage of the versatile linguistic knowledge of Pre-trained Language Model, resulting in competitive accuracy compared with recent baselines. The WordTransABSA demonstrates its superiority and effectiveness through extensive experiments in both data-sufficient (full-data supervised learning) and data-insufficient (few-shot learning) scenarios. We have made our code publicly available on GitHub: https://github.com/albert-jin/WordTransABSA.

Keywords: Natural Language Processing; Aspect-based Sentiment Analysis; Masked Language Model; Pre-trained Language Model; Few-shot supervised learning.
