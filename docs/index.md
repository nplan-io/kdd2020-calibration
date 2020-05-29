---
layout: default
---

<h1>How to calibrate your neural network classifier</h1>
<h2>Getting true probabilities from a classification model</h2>

For a long time, machine learning professionals have optimised for accuracy when training 
classification models. However, in recent years, focus has begun to shift towards using models 
whose predictions can be meaningfully used as probabilities.

When practitioners want to measure the model's confidence in its predictions, they often try using 
its softmax output, although this usually does not represent the true probabilistic distribution. 
These models, where the softmax is biased towards either under- or over-confidence in its predictions, 
are called "uncalibrated". Models that fail to take this into account can be dangerous, especially 
when the stakes are high.

To help you learn how to avoid these mistakes, we will use a pre-trained model to demonstrate some 
visual tools and metrics to understand how well calibrated your classification model is and demonstrate 
ways to calibrate the model after training - from theory to a Keras implementation.

<h3>Presenters</h3>
<div class="photo-container">
<figure>
    <img src="/assets/image/natalia.jpg" alt="Natalia Culakova" width="45%" class="blackandwhite">
    <figcaption>Natalia Culakova, nPlan</figcaption>
</figure> <figure>
    <img src="/assets/image/dan.jpg" alt="Dan Murphy" width="45%" class="blackandwhite"/>
    <figcaption>Dan Murphy, nPlan</figcaption>
</figure> 
</div>

<!--```python
calibrate.model('metadata.yaml')
```-->
