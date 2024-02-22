---
title: "Prompt learning for metonymy resolution: Enhancing performance with internal prior knowledge of pre-trained language models"
collection: publications
permalink: /publication/2023-08-23-knosys-promptMR
excerpt: 'This paper is about the Prompt learning for metonymy resolution task.'
date: 2023-08-23
venue: 'Knowledge-Based Systems'
paperurl: 'https://doi.org/10.1016/j.knosys.2023.110928'
citation: 'Biao Zhao and Weiqiang Jin et al. (2023). &quot;Prompt learning for metonymy resolution: Enhancing performance with internal prior knowledge of pre-trained language models.&quot; <i>Knowledge-Based Systems</i>. Volume 279, 2023, 110928, ISSN 0950-7051.'
---

Linguistic metonymy is a common type of figurative language in natural language processing (NLP), where a concept is represented by a closely associated word or phrase, for example “business executives suits”. As a result, metonymy resolution has become an important NLP task aimed at correctly identifying metonymic expressions within sentences. Previous approaches to this task have typically relied on pre-trained language models (PLMs) using a fine-tuning process. However, this can be time-consuming and resource-intensive, and may lead to a loss of factual prior knowledge. The emergence of a novel learning paradigm termed “prompt learning” or “prompt-tuning” has recently sparked widespread interest and captured considerable attention, as it has proven to yield remarkable results and surpass previous benchmarks. This approach uses a “pre-train→prompt→predict” paradigm and has been shown to better utilize the internal prior knowledge of a PLM, especially in situations with limited supervised resources. Inspired by this success, we investigated how prompt learning could improve metonymy resolution. We have developed a series of prompt learning approaches, called PromptMR, for metonymy resolution, and applied them to several widely-used metonymy resolution datasets. We also designed additional prompt-tuning augmentation strategies to further enhance the potential of prompt learning. Our experiments demonstrated that our method achieved state-of-the-art performance over multiple competitive baselines in both data-sufficient and data-scarce scenarios. The code implementations for PromptMR are accessible on GitHub via the URL: https://github.com/albert-jin/PromptTuning2MetonymyResolution.

Keywords: Metonymy resolution; Prompt learning; Pre-trained language model; Prompting template engineering; Answer engineering.
