# How to calibrate your neural network classifier: 
## Getting accurate probabilities from a classification model

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
1. What is model calibration and why do we need it?
2. How to measure calibration?
  * Reliability diagrams
  * Expected calibration error
  * Maximum calibration error
  * nPlan’s RMS calibration error
  * Adapting these to multiclass problems
3. How to calibrate classification models?
  * Temperature scaling
  * Platt scaling
  * Matrix and vector scaling
4. How can we use this in real life situations?
