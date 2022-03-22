---
layout: single
title: "Research"
permalink: /research/
---

## Publications

[Google Scholar](https://scholar.google.fr/citations?hl=fr&user=mG6V3q4AAAAJ&view_op=list_works&sortby=pubdate)


## Machine Learning with Structured Sparsity

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
