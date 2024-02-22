---
title: "Back to common sense: Oxford dictionary descriptive knowledge augmentation for aspect-based sentiment analysis"
collection: publications
permalink: /publication/2023-01-04-ipm-DictABSA
excerpt: 'This paper is about Knowledge Enhancement on Aspect-based Sentiment Analysis (ABSA).'
date: 2023-01-04
venue: 'Information Processing & Management (ipm)'
paperurl: 'https://doi.org/10.1016/j.ipm.2022.103260'
citation: 'Weiqiang Jin et al. (2023). &quot;Back to common sense: Oxford dictionary descriptive knowledge augmentation for aspect-based sentiment analysis.&quot; <i>Information Processing & Management</i>. Volume 60, Issue 3, 2023, 103260, ISSN 0306-4573.'
---

Aspect-based Sentiment Analysis (ABSA) is a crucial natural language understanding (NLU) research field which aims to accurately recognize reviewers’ opinions on different aspects of products and services. Despite the prominence of recent ABSA applications, mainstream ABSA approaches inevitably rely on large-scale supervised corpora, and their final performances is susceptible to the quality of the training datasets. However, annotating sufficient data is labour intensive, which presents a significant barrier for generalizing a high-quality sentiment analysis model. Nonetheless, humans can make more accurate judgement based on their external background knowledge, such as factoid triples knowledge and event causality. Inspired by the investigations on external knowledge enhancement strategies in other popular NLP research, we propose a novel knowledge augmentation framework for ABSA, named the Oxford Dictionary descriptive knowledge-infused aspect-based sentiment analysis (DictABSA). Comprehensive experiments with many state-of-the-art approaches on several widely used benchmarks demonstrate that our proposed DictABSA significantly outperforms previous mainstream ABSA methods. For instance, compared with the baselines, our BERT-based knowledge infusion strategy achieves a substantial 6.42% and 5.26% absolute accuracy gain when adopting BERT-SPC on SemEval2014 and ABSA-DeBERTa on ACLShortData, respectively. Furthermore, to effectively make use of dictionary knowledge we devise several alternative knowledge infusion strategies. Extensive experiments using different knowledge infused strategies further demonstrate that the proposed knowledge infusion strategies effectively enhance the sentiment polarity identification capability. The Python implementation of our DictABSA is publicly available at https://github.com/albert-jin/DictionaryFused-E2E-ABSA.

Additional Key Words and Phrases: Natural language understanding; Aspect-based sentiment analysis; Knowledge infusion mechanisms; Pre-trained language models; Model hot-plugging technique.
