---
title: "A semi-independent policies training method with shared representation for heterogeneous multi-agents reinforcement learning"
collection: publications
permalink: /publication/2023-06-19-fnins-MARL
excerpt: 'This paper is about multi-agents reinforcement learning (MARL).'
date: 2023-06-19
venue: 'Frontiers in Neuroscience'
paperurl: 'https://doi.org/10.3389/fnins.2023.1201370'
citation: 'Biao Zhao and Weiqiang Jin et al. (2023). &quot;A semi-independent policies training method with shared representation for heterogeneous multi-agents reinforcement learning.&quot; <i>Frontiers in Neuroscience</i>. Volume 17, 2023, 1201370, ISSN 1662-453X.'
---

Humans do not learn everything from the scratch but can connect and associate the upcoming information with the exchanged experience and known knowledge. Such an idea can be extended to cooperated multi-reinforcement learning and has achieved its success on homogeneous agents by means of parameter sharing. However, it is difficult to straightforwardly apply parameter sharing when dealing with heterogeneous agents thanks to their individual forms of input/output and their diverse functions and targets. Neuroscience has provided evidence that our brain creates several levels of experience and knowledge-sharing mechanisms that not only exchange similar experiences but also allow for sharing of abstract concepts to handle unfamiliar situations that others have already encountered. Inspired by such a brain's functions, we propose a semi-independent training policy method that can well tackle the conflict between parameter sharing and specialized training for heterogeneous agents. It employs a shared common representation for both observation and action, enabling the integration of various input and output sources. Additionally, a shared latent space is utilized to maintain a balanced relationship between the upstream policy and downstream functions, benefiting each individual agent's target. From the experiments, it can approve that our proposed method outperforms the current mainstream algorithms, especially when handling heterogeneous agents. Empirically, our proposed method can also be improved as a more general and fundamental heterogeneous agents' reinforcement learning structure for curriculum learning and representation transfer. All our code is open and released on https://gitlab.com/reinforcement/ntype.

Keywords: brain function, knowledge-sharing institution, multi-agent reinforcement learning, parameters sharing, representation transferability.
