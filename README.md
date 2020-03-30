# How to calibrate your neural network classifier
## Getting true probabilities from a classification model

### Setup
1. Download Python 3.6 or later https://www.python.org/downloads/

2. Install Jupyter Notebook https://jupyter.org/install

3. Clone this repository https://help.github.com/en/github/creating-cloning-and-archiving-repositories/cloning-a-repository

4. Install necessary libraries from the requirements.txt

With pip `pip3 install -r requirements.txt`

With conda `conda install --file requirements.txt`

5. Test run jupyter notebook

In terminal or cmd by running `jupyter notebook` the jupyter notebook environment will appear in your browser tab
or alternatively within your prefered Python IDE (Pycharm, VSCode, ..)

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
