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

More than 530 million people globally suffer from diabetes, a leading cause of death and contributor to a host of long-term serious health complications. To treat diabetes, individuals need to manage their blood glucose level through diet, exercise, weight loss and medications. Many people with diabetes, in particular with Type I diabetes, require frequent insulin injections throughout the day to maintain a healthy glucose profile.

Frequently measuring glucose, for example through continuous glucose monitoring (CGM) devices, is therefore a crucial component of diabetes care. CGMs are small wearable devices widely used by people with diabetes to continuously monitor their blood glucose levels. They provide valuable information that help patients make informed decisions about their diet and insulin dosing. However, control of blood sugar levels remains challenging, as a myriad of complex factors influence the dynamics of a patient's glucose profile, including cardiometabolic risk factors such as obesity, age, sex, or exercise. These complex relationships are not yet fully understood, but they will need to be incorporated for effective next generation treatment systems.

Our research interests include:

- Transformer-based approaches for training large CGM models
- Glucose forecasting
- Cardiometabolic risk factor prediction and biomarker discovery


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/research/cgm" title="Research area: analysing CGM data" class="img-fluid rounded z-depth-1" %}
    </div>
</div>


### Interpretable methods for diabetic retinopathy detection

Deep learning models typically lack interpretability, thereby posing ethical concerns and preventing wide adoption in clinical practice. Interpreting deep learning models typically relies on post-hoc saliency map techniques. However, these techniques often fail to serve as actionable feedback to clinicians, and they do not directly explain the decision mechanism. In our research, we are interested in two approaches to mitigate the shortcomings saliency maps:

1. Inherently interpretable models, which combine the feature extraction capabilities of deep neural networks with advantages of sparse linear models in interpretability. 

2. Visual counterfactual explanations, which provide realistic counterfactuals ("what would this image have looked like, were the patient healthy?") to illustrate a ML model's internal reasoning.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/research/kerol_bagnets" title="Research area: interpretable ML" class="img-fluid rounded z-depth-1" %}
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