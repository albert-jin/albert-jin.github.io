---
title: "Relation-aware graph structure embedding with co-contrastive learning for drug–drug interaction prediction"
collection: publications
permalink: /publication/2024-01-05-neucom-RaGSECo
excerpt: 'This paper is about drug–drug interactions (DDIs).'
date: 2024-01-05
venue: 'Neurocomputing (neucom)'
paperurl: 'https://doi.org/10.1016/j.neucom.2023.127203'
citation: 'Mengying Jiang, Guizhong Liu, Biao Zhao, Yuanchao Su, Weiqiang Jin. (2023). &quot;Relation-aware graph structure embedding with co-contrastive learning for drug–drug interaction prediction.&quot; <i>Neurocomputing</i>. Volume 572, 2024, 127203, ISSN 0925-2312.'
---

Relation-aware graph structure embedding (RaGSE) is promising for predicting multi-relational drug–drug interactions (DDIs). Most existing methods based on RaGSE commence by constructing a multi-relational DDI graph. They then learn the RaGSEs for drugs by aggregating their neighbor’s features under different relations. Nevertheless, new drugs lack neighbors in the DDI graph. This limitation hinders the ability of these methods to effectively learn RaGSEs for new drugs, resulting in suboptimal performance when evaluating DDIs that involve new drugs. To alleviate this issue, we propose a novel DDI prediction method based on relation-aware graph structure embedding with co-contrastive learning, RaGSECo. The proposed RaGSECo constructs two heterogeneous graphs: a multi-relational DDI graph and a multi-attribute drug–drug similarity (DDS) graph. The two graphs are used respectively for learning and propagating the RaGSEs of drugs, aiming to ensure all drugs, including new ones, can possess effective RaGSEs. Additionally, we present a novel co-contrastive learning module to learn feature representations for drug pairs (DPs). This module learns DP representations from two distinct views (interaction and similarity views) and encourages these views to supervise each other collaboratively to obtain more discriminative DP representations. We evaluate the effectiveness of our RaGSECo on three different tasks using two real datasets. Experimental outcomes unequivocally indicate that our RaGSECo surpasses several state-of-the-art methods in performance.

Additional Key Words and Phrases: Adverse drug reactions; Graph neural networks; Graph structure embedding; Self-supervised learning.
