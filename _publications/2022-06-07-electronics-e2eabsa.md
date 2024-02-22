---
title: "A Novel Cascade Model for End-to-End Aspect-Based Social Comment Sentiment Analysis"
collection: publications
permalink: /publication/2022-06-07-electronics-e2eabsa
excerpt: 'This paper is about end-to-end aspect-based social comment sentiment analysis (E2E-ABSA) task.'
date: 2022-06-07
venue: 'the Special Issue Intelligent Implementations in the Digitalized Real World of Journal Electronics'
paperurl: 'https://doi.org/10.3390/electronics11121810'
citation: 'Hengbing Ding; Shan Huang; Weiqiang Jin; Yuan Shan; Hang Yu. (2022). &quot;A Novel Cascade Model for End-to-End Aspect-Based Social Comment Sentiment Analysis.&quot; <i>Electronics</i>. 2022; 11(12):1810.'
---

The end-to-end aspect-based social comment sentiment analysis (E2E-ABSA) task aims to discover human’s fine-grained sentimental polarity, which can be refined to determine the attitude in response to an object revealed in a social user’s textual description. The E2E-ABSA problem includes two sub-tasks, i.e., opinion target extraction and target sentiment identification. However, most previous methods always tend to model these two tasks independently, which inevitably hinders the overall practical performance. This paper investigates the critical collaborative signals between these two sub-tasks and thus proposes a novel cascade social comment sentiment analysis model for jointly tackling the E2E-ABSA problem, namely CasNSA. Instead of treating the opinion target extraction and target sentiment identification as discrete procedures in previous works, our new framework takes the contextualized target semantic encoding into consideration to yield better sentimental polarity judgment. Additionally, extensive empirical results show that the proposed approach effectively achieves a 68.13% F1-score on SemEval-2014, 62.34% F1-Score on SemEval-2015, 56.40% F1-Score on SemEval-2016, and 50.05% F1-score on a Twitter dataset, which is higher than the existing approaches. Ablated experiments demonstrate that the CasNSA model substantially outperforms state-of-the-art methods, even when using fixed words embedding rather than pre-trained BERT fine tuning. Moreover, in-depth performance analysis on the social comment datasets further validates that our work gains superior performance and reliability effectively and efficiently in realistic scenarios.

Additional Key Words and Phrases: machine learning; natural language processing; fine-grained sentiment analysis; fine-tuning transformer BERT; multi-level cascade tagging scheme.
