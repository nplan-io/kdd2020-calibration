# How to calibrate your neural network classifier
## Getting true probabilities from a classification model

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
* nPlan’s RMS calibration error
3. Methods for calibrating classifiers:
* Temperature scaling
* Platt scaling
* Matrix and vector scaling
4. How is calibration used in the real world?
