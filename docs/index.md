---
layout: default
---

<h2>How to calibrate your neural network classifier</h2>
<h3>Getting true probabilities from a classification model</h3>

When training classification models, machine learning professionals often optimise for accuracy 
and other related metrics. Greater accuracy has been the focus of machine learning papers for 
many years, with results often reported in terms of metrics like accuracy and F1 score on standard 
datasets, such as MNIST, CIFAR 10, 100, and ImageNet. However, in recent years, focus has begun to 
shift towards using models whose predictions can be meaningfully used as probabilities.

There are cases when a practitioner already has a trained classification model and would like to 
extract from it a measure of confidence in its predictions. One (naive) method may be to interpret 
a model’s softmax output as the model’s estimation of the likelihood that the classification is 
correct. 

We will show that using this method often does not represent the true probabilistic distribution. 
We call models like this “uncalibrated” - that is, the softmax output is biased towards either 
under- or over-confidence in its predictions.

Models that fail to take this into account are dangerous, especially when the stakes are high, 
like modelling the likelihood of a person being ill. An overconfident model can send an infectious 
patient home to their family or unnecessarily allocate resources to a healthy individual, instead 
of referring them to a human physician.

To avoid mistakes like this, we will use a pre-trained model to demonstrate some visual tools 
that help you understand how well calibrated your classification model is. We will then explore 
some metrics to measure the size of the calibration problem in a binary setting, extend them to a 
multiclass setting, and demonstrate ways to calibrate the model after training - from theory to a 
Keras implementation.

<h3> Presenters </h3>
![Natalia Culakova](/assets/image/natalia.jpg)  |  ![Dan Murphy](/assets/image/dan.jpg)
Natalia Culakova, nPlan | Dan Murphy, nPlan

<!--```python
calibrate.model('metadata.yaml')
```-->
