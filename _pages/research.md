---
layout: single
title: "Research"
permalink: /research/
---

## Publications

[Google Scholar](https://scholar.google.com/citations?user=3GelV-YAAAAJ&hl=en)

## Boosting Prior Knowledge in Machine Learning for Biomarker Discovery
The so-called **small n, large p** problem makes learning classification or regression models difficult for biomedical applications. In such a problem especially in clinical dataset, adding samples is not easy so feature selection or embedding techniques should be used to reduce the number of features *p*. Prior knowledge is fundamentally important and relevant information that can provide an efficient way to regularize the number of features for training machine learning models. Because these knowledge comes from accumulated studies of various biological systems, it is also applicable to patients and model organisms.

In this study, we tried to prevent overfitting of the model and improve the robustness of the model by iteratively querying the appropriateness of the features for each model training process.

### Disease Gene Prioritization for Classification (DGP4C)
Disease gene prioritization methods such as network propagation and similarity profiling have been used to prioritize candidate disease genes for experimental validation. However, it is not clear whether these disease gene prioritization methods can be used as feature selection techniques for gene expression-based disease classification models. In this study, we developed and validated a method for prioritizing disease genes that shows high importance for the classification of disease phenotypes. 



![Figure1. Schematic of Disease Gene Prioritization for Classification (DGP4C) Framework](/profile/images/dgp4c.jpg)

<p><strong> Figure1. Schematic of Disease Gene Prioritization for Classification (DGP4C) Framework </strong></p>

Figure 1 provides a schematic diagram of the proposed DGP4C framework. The algorithm begins finding candidate disease genes using a disease gene prioritization method based on a combination of disease gene scores calculated from network propagation and function similarity profiling. The feature importance of candidate disease genes for disease phenotype classification is then assessed and important candidate genes are fed back to the gene prioritization step to update candidate disease genes until no additional disease gene candidates are found.

![Figure2. Performance Assessment of Disease Gene Prioritization for Classification (DGP4C) Framework](/profile/images/dgp4c_result.jpg)

<p><strong> Figure2. Performance Assessment of Disease Gene Prioritization for Classification (DGP4C) Framework </strong></p>



Figure 2 shows performance evaluation result of DGP4C algorithm in Neo-Adjuvant Chemotherapy (NAC) response prediction in breast cancer. As expected, DGP4C showed best performance compared to all other non-iterative approach to optimize gene expression markerset. 


### Disease Mechanism Subgroup Identification by Iterative Error Estimation (DMSDIE)

### Random Subsample Subspace Ensemble (RDSE)



## Self-Supervised Learning for reproducible research
The self-supervised Learning (SSL) is defined as a machine learning strategy that can be supervised by the transformed training features rather than labels. Self-supervised learning is especially useful when the measurement or labeling process involves uncertainty. In biomedical dataset as well as biosignal processing, many problems can be formulated as self-supervised learning problems. 

### Minimum Variance Representation Learning (MVNet)




## Sparse Representation Learning

### Deep Latent Space Encoding (DeepLSE)

### Deep Sparse Reconstruction Classifier (DeepSRC)



## Ovelap Statistics and its applications

### Ovltools: an R package for estimation of arbitrary distribution overlap

### GMDM: Generalized Multi-Dimensional overlap Metric



<!--
## Generative Adversarial Network (GAN) for Biomedical Signal Processing Applications

### Batch-effect Minimization Network (BatchGAN)

### Platform Transformer Network (PTN)

### Drug Response Prediction using Adaptive Instance Normalization (DRAdaIN)

-->

<!--
The use of machine-learning in neuroimaging offers new perspectives in early diagnosis and prognosis of brain diseases. However, algorithms should provide interpretable solutions. Biomarkers identification based on neuroimaging require new algorithms that exploit the natural spatial structure of the brain images.

Although such multivariate methods can capture complex relationships in the data, traditional approaches provide irregular or scattered (l1 penalty, see Lasso penalty the figure below) predictive pattern with a very limited relevance.
![weight_map_adni_3d_enet](/images/weight_map_adni_3d_enet.png "Logo Title Text 1")

Essentially, we propose to extend state-of-the-art algorithms (such Elastic-net) with biolological priors to force the produced solution to adhere to some domain-specific constraints. More precisely, our first aim is to exploit the known spatial structure of the neuroimaging data that stem from meshes of cortical surface or 3D grid (volume) of the brain.

A penalty like Total Variation (TV) that exploits the natural 3D structure of the images can increase the spatial coherence of the weight map.
![weight_map_adni_3d_enettv](/images/weight_map_adni_3d_enettv.png "Logo Title Text 1")

**Generalization to any type of data with spatial structure, for instance meshes of the cortical surface**

The algorithms are based on a versatile mathematical framework which authorizes a straightforward application on any type of structured input data: 3 dimensional image or meshes of the cortical surface.
The next figure shows the weights map obtained by a classic Lasso-based algorithms on mesh of cortical thickness.
![weight_map_adni_mesh_enet](/images/weight_map_adni_mesh_enet.png "Logo Title Text 1")

The next figure shows the weights map obtained by adding a TV penalty.
![weight_map_adni_mesh_enettv](/images/weight_map_adni_mesh_enettv.png "Logo Title Text 1")

Structured sparsity based on TV provides **interpretable and stable** predictive brain maps.

However, TV penalization leads to non-smooth optimization problems which disables classical gradient descent methods.


**Optimization**

Within the BrainOmics team at NeuroSpin, we developed an optimization framework that minimizes any combination of l1, l2, and TV penalties while preserving the exact l1 penalty. This algorithm uses Nesterov's smoothing technique to approximate the TV penalty with a smooth function such that the loss and the penalties are minimized with an exact accelerated proximal gradient algorithm. We propose an original continuation algorithm that uses successively smaller values of the smoothing parameter to reach a prescribed precision while achieving the best possible convergence rate. This algorithm (CONESTA: COntinuation with NEsterov smoothing in a Shrinkage Thresholding Algorithm) can be used with other losses or penalties.
ParsimonY: Sparse and Structured Machine Learning Libray in Python
With The BrainOmics(*) team,  we produced a library [ParsimonY on github](https://github.com/neurospin/pylearn-parsimony) based on the python language that implements many structured machine learning algorithms. The first stable release is scheduled by mid May 2014.


**BrainOmics team at NeuroSpin in 2015:**

- Vincent Frouin (Head of the team)
- Fouad Hadj Selem (Post-doc)
- Tommy Lofstedt (Post-doc)
- Mathieu Dubois (Post-doc)
- Jinpeng Li (Research Engineer)

-->