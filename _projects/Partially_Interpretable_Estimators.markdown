---
layout: page
title: Partially Interpretable Estimators (PIE)
description: PIE model is a new form of predictive model that boost predictive performance while maintaining interpretability
img:
importance: 1
category: Interpretability
status: under review
keywords: [interpretability, hybrid model]
---
<style>
  body {
  text-align: justify}
  </style>

<h4><b>Abstract</b></h4>

We propose a new form of a predictive model, Partially Interpretable Estimators (PIE). A PIE model attributes a prediction to individual features via an interpretable model, while the remaining of the PIE prediction is captured by a black-box model, with the goal to boost the predictive performance while maintaining interpretability. As such, the interpretable model  captures the main contributions of features,  and the black-box model complements the interpretable piece by capturing the “nuances” of feature interactions as a refinement. We also include a sparsity constraint such that users can tune the model to meet domain-specific requirements of interpretability. We design a coordinated training algorithm to jointly train the two types of models to globally optimize the performance and achieve the best collaboration of the two. Experimental results show that PIE is highly competitive to state-of-the-art black-box models on tabular data. In addition,the understandability of PIE is comparable to linear models as validated via human evaluations.

<strong>Codes for PIE model is in <a href="https://github.com/MissTiny/Partially-Interpretable-Estimators" target="_blank">GitHub</a>. </strong>

<div class="d-flex justify-content-center">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/project_PIE/PIE_model_image.png' | relative_url }}" alt="" title="example image"/>

</div>
<div class="caption">
    The simple explaination of PIE model.
</div>

<strong>For detailed functions, such as objective functions, please check the pre-print paper <a href="https://arxiv.org/abs/2105.02410" target="_blank">here</a>.</strong>
