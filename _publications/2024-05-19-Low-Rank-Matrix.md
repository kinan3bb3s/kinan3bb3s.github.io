---
title: "Locally-Rank-One-Based Joint Unmixing and Demosaicing Methods for Snapshot Spectral Images. Part I: a Matrix-Completion Framework"
collection: publications
permalink: /publication/2024-01-01-locally-rank-one-based-joint-unmixing-and-demosaicing-methods-for-snapshot-spectral-images
category: "Journal Articles"
excerpt: 'This article presents a matrix-completion framework for locally-rank-one-based joint unmixing and demosaicing methods, focusing on advancements in snapshot spectral imaging.'
date: 2024-05-19
venue: 'IEEE Transactions on Computational Imaging'
slidesurl: ''  # Add URL if slides or presentation materials are available
paperurl: 'https://ieeexplore.ieee.org/document/10535266'  # Add URL if the paper is available online
citation: 'Abbas, Kinan, Puigt, Matthieu, Delmaire, Gilles, and Roussel, Gilles. (2024). &quot;Locally-Rank-One-Based Joint Unmixing and Demosaicing Methods for Snapshot Spectral Images. Part I: a Matrix-Completion Framework.&quot; <i>IEEE Transactions on Computational Imaging</i>,  vol. 10, pp. 848-862, 2024.'
author_version: 'TCI.2024.3402322.pdf'  # Point to the file in the files folder


---

With the recent advancements in design and processing speed, a new snapshot mosaic imaging sensor architecture (SSI) has been successfully developed, holding the potential to transform the way dynamic scenes are captured using miniaturized platforms. However, SSI systems encounter a core trade-off concerning spatial and spectral resolution due to the assignment of individual spectral bands to each pixel. While the SSI camera manufacturer provides a pipeline to process such data, we propose in this paper to process the RAW SSI data directly. We show this strategy to be much more accurate than post-processing after the pipeline. In particular, in the first part of this paper, we propose a low-rank matrix factorization and completion framework which jointly tackles both the demosaicing and the unmixing steps of the SSI data. In addition to a “natural” technique, we expand the well-known pure pixel assumption to the SSI sensor level and propose two dedicated methods to extract the endmembers. The first one can be seen as a weighted Sparse Component Analysis (SCA) method, while the second one relaxes the abundance sparsity assumption of the former. The abundances are then recovered by applying the naive approach with the fixed extracted endmembers. Finally, we experimentally validate the merits of the proposed methods using synthetically generated data and real images obtained with an SSI camera.