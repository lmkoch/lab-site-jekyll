---
layout: page
permalink: /research/
title: research
description: Our research interests.
nav: true
nav_order: 2
# related_publications: true
---


Methodological interests in trustworthy AI:

- Interpretable machine learning
- Performance generalisation and performance prediction
- Subgroup discovery
- Disentangled representation learning

Application areas:

- Medical image analysis including for example image classification, segmentation, disease progression modelling
- Interpretation of Continuous Glucose Monitoring (CGM) data, including for example CGM forecasting and risk factor prediction


Check out some example projects (past and ongoing) below. For a comprehensive list of publications, check out [google scholar](https://scholar.google.com/citations?user=R0iwuiIAAAAJ).



### Subgroup discovery for monitoring ML performance in hidden stratifications

Traditional subgroup analysis, a common practice in medical research, often falls short when evaluating deep learning models for medical imaging.  Although useful, this practice masks significant performance variations among specific groups. Clinical trials and medical AI studies often stratify results by demographic attributes (e.g., age, sex, or ethnicity), but AI medical models might not rely on these standard metadata categories, leading to suboptimal performance evaluations.

We study an alternative approach: using subgroup discovery methods to enrich performance analysis. Subgroup discovery methods uncover hidden patterns and systematic groupings beyond traditional metadata, providing deeper and more meaningful insights into AI model performance.  We have many challenges to overcome, in special validation of subgroup discovery, as labels for ground truth inherently do not exist in real data. We argue that subgroup discovery can be an effective and easily implemented tool to enhance the performance validation and monitoring of ML systems in medicine.


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/research/alceu_subgroups.png" title="Research area: subgroup discovery" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

- {% reference bissoto2025subgroup --file refs_website.bib %}


### Simulation-Based Inference for digital twins in Type 1 Diabetes


Type 1 Diabetes (T1D) affects over 9 million people worldwide and requires frequent insulin injections and continuous monitoring of blood glucose levels with wearable continuous glucose monitoring (CGM) devices. The dynamics between glucose, meal intake, and insulin over time can be described by complex physiological models consisting of systems of differential equations, where model parameters (e.g., insulin sensitivity) can be highly patient-specific. Identifying these parameters from observed data enables the creation of a digital twin (DT) of an individual’s metabolic system, supporting treatment planning, prediction, and real-time adaptation.

Parameter estimation in such models is a challenging inverse problem. Existing approaches, such as Markov Chain Monte Carlo (MCMC), are computationally expensive, non-amortized, and often rely on steady-state initial condition assumptions that may not hold in practice. Therefore, we are working on Simulation-Based Inference (SBI) method based on Neural Posterior Estimation (NPE), which enables efficient inference of both physiological parameters and initial conditions. Unlike traditional methods, SBI provides fast, amortized inference and produces full posterior distributions, allowing uncertainty quantification and more reliable decision-making. Future extensions will explore robustness to model misspecification and missing CGM data.



<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/research/trung_sbi.png" title="Research area: simulation-based inference in diabetes" class="img-fluid w-50 d-block mx-auto rounded z-depth-1" %}
    </div>
</div>

- {% reference hoang2025simulation --file refs_website.bib %}


### Distribution shift detection for postmarket surveillance of medical AI algorithms

Distribution shifts remain a problem for the safe application of regulated medical AI systems, and may impact their real-world performance if undetected. Postmarket shifts can occur for example if algorithms developed on data from various acquisition settings and a heterogeneous population are predominantly applied in hospitals with lower quality data acquisition or other centre-specific acquisition factors, or where some ethnicities are over-represented. Therefore, distribution shift detection could be important for monitoring AI-based medical products during postmarket surveillance. We investigated, implemented and evaluated various deep-learning based shift detection techniques on simulated shifts in medical imaging datasets. We then simulated population shifts and data acquisition shifts and analysed the performance of the shift detectors at detecting both subgroup and out-of-distribution shifts.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/research/lisa_subgroups.png" title="Research area: distribution shift detection" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

- {% reference koch2024postmarket --file refs_website.bib %}
- {% reference koch2022hidden --file refs_website.bib %}



### Timeseries transformers for analysing continuous glucose monitoring data

To treat diabetes, individuals need to manage their blood glucose level through diet, exercise, weight loss and medications. Many people with diabetes, in particular with Type I diabetes, require frequent insulin injections throughout the day to maintain a healthy glucose profile.

Frequently measuring glucose, for example through continuous glucose monitoring (CGM) devices, is therefore a crucial component of diabetes care. CGMs are small wearable devices widely used by people with diabetes to continuously monitor their blood glucose levels. They provide valuable information that help patients make informed decisions about their diet and insulin dosing. However, control of blood sugar levels remains challenging, as a myriad of complex factors influence the dynamics of a patient's glucose profile, including cardiometabolic risk factors such as obesity, age, sex, or exercise. These complex relationships are not yet fully understood, but they will need to be incorporated for effective next generation treatment systems.

Our research interests include:

- Transformer-based approaches for training large CGM models
- Glucose forecasting
- Cardiometabolic risk factor prediction and biomarker discovery


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/research/cgm.png" title="Research area: analysing CGM data" class="img-fluid rounded z-depth-1" %}
    </div>
</div>


### Interpretable methods for diabetic retinopathy detection

Deep learning models typically lack interpretability, thereby posing ethical concerns and preventing wide adoption in clinical practice. Interpreting deep learning models typically relies on post-hoc saliency map techniques. However, these techniques often fail to serve as actionable feedback to clinicians, and they do not directly explain the decision mechanism. In our research, we are interested in two approaches to mitigate the shortcomings saliency maps:

1. Inherently interpretable models, which combine the feature extraction capabilities of deep neural networks with advantages of sparse linear models in interpretability. 

2. Visual counterfactual explanations, which provide realistic counterfactuals ("what would this image have looked like, were the patient healthy?") to illustrate a ML model's internal reasoning.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/research/kerol_bagnets.png" title="Research area: interpretable ML" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<!-- <div class="caption">
    This image can also have a caption. It's like magic.
</div> -->

Relevant publications:


- {% reference djoumessi2023sparse --file refs_website.bib %}
- {% reference sun2023right --file refs_website.bib %}
- {% reference sun2023inherently --file refs_website.bib %}
- {% reference boreiko2022visual --file refs_website.bib %}



<!-- ### Performance prediction

(Patrick)

### Disentangled representation learning

(Sarah) -->