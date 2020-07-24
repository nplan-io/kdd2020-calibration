# How to calibrate your neural network classifier
## Getting true probabilities from a classification model

This is a repository for a hands-on tutorial on calibration at the KDD 2020 virtual conference. 
It comprises of slides to explain some concepts, resources for further reading and template colab 
notebook for those who want to try implementing some of these methods, as well as some model answers.
This tutorial will be shared as a video for the virtual conference and later accessible on youtube.

### Setup
0. Ensure you have an up to date browser installed (ideally Chrome, Firefox or Safari)

1. Click this link to take you to [the notebook template](https://colab.research.google.com/github/nplan-io/kdd2020-calibration/blob/master/tutorial/KDD%202020%20-%20nPlan%20calibration%20session.ipynb)

2. At the end of the tutorial, follow this link to take you to some [model answers](https://colab.research.google.com/github/nplan-io/kdd2020-calibration/blob/master/tutorial/KDD%202020%20-%20nPlan%20calibration%20session%20(completed).ipynb)

### Tutorial outline
1. Overview of calibration:
    * What is model calibration?
    * When to use calibration
    * Pitfalls of not considering calibration

2. Measuring calibration (in Python):
    * Reliability diagrams
    * Expected calibration error
    * Maximum calibration error
    * RMS calibration error
3. Literature review
    * Platt, J. - Probabilistic outputs for support vector machines and comparisons to regularized likelihood methods
    * Niculescu-Mizil, Alexandru & Caruana, Rich. - Predicting good probabilities with supervised learning
    * Guo, C., Pleiss, G., Sun, Y., & Weinberger, K. Q. - On calibration of modern neural networks 

4. Methods for calibrating classifiers:
    * Isotonic regression
    * Platt scaling
    * Temperature scaling
    * Matrix and vector scaling

5. How is calibration used in the real world?
