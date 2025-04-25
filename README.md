# mlsec-project
Project 2 for Machine Learning Security, by Jules COOPER and Leonie MAIER

## Setup
The project requires python version 3.10, and the libraries indicated in requirements.txt
It also requires to download models from RobustBench, which can be downloaded through the code cells or done manually and placed in a /models/ folder.

## Description
This project crafts adverserial examples on 3 models from RobustBench and tests the transferability on 7 other models.

### statistical_multi_run.ipynb
This is the code that has been run to compute statistics on the performance of the attack and their transferability, by running 100 attacks on 2 different ensembles of models. Each successful adversarial example was then tested on 7 other individual models. It requires a very long computing time (8+ hours), due to the heavier models in the second ensemble.

### demo_single_example.ipynb
This is a simplified version of the previous code, where the goal is to find only one adversarial example on the more lightweight ensemble of models. This single adversarial example is then presented to the same 7 other models. This requires a much shorter computing time (<15min).
