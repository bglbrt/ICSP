# ICSP | Information and Complexity SimulationsPlus Data Challenge

This repository contains our attempts at the 2022 ENS | SimulationsPlus Data Challenge.

The task of the challenge is that of obtaining the lowest mean-squared error (MSE) in a regression problem relating experimentally obtained properties of chemical compounds to an undisclosed variable closely related to the ADMET properties of the compounds. We propose two ways to address this challenge:
- one, prediction-oriented, using a kernel ridge regression with Laplacian kernel which achieves a MSE of 0.0323 on the public test dataset;
- another which takes its roots in causal inference theory, and which achieves a MSE of 0.0302 on the public test dataset, and of 0.0297 on the private test dataset. Both of these approaches beat the baseline provided with the challenge by an extensive margin

## Data

Data used to train and evaluate the algorithm consists in the data provided by the challenge organisers:
- `input_training.csv`
- `input_testing.csv`
- `output_training.csv`

No additional data was used to obtain the results displayed above. The data is not included in this repository but can be found on the [website](https://challengedata.ens.fr) of the challenge.

## Usage

To reproduce these results, please start by cloning the repository locally:

```
git clone https://github.com/bglbrt/SSPSP.git
```

Then, install the required libraries:

```
pip install -r requirements.txt
```

All files can be run as `.ipynb` files in a Jupyter environment.

## Required libraries

The files present on this repository require the following libraries (also listed in requirements.txt):
 - [NumPy](https://numpy.org)
 - [torch](https://pytorch.org)
 - [matplotlib](https://matplotlib.org)
