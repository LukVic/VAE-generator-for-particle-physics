# A synthetic data generator for particle physics using variational autoencoders
In this project, we augmented Monte-Carlo simulated data for charged Higgs boson searches. Events are selected if they have two light leptons (electron or muon) of the same sign and exactly one hadronically decaying tau-lepton. For the data generation, a variational autoencoder model was used with evidence lower bound and symmetric equilibrium learning. Both mentioned learning approaches were also tested with hierarchical (Ladder) archi- tecture. For the data quality assessment, both qualitative and quantitative metrics were taken into account. The standard evidence lower bound (ELBO) learning model was selected as the best-performing option. The model was then used to generate data for the signal and background separation analysis experiments. The dependence of classifier performance on the training dataset size was demonstrated using two widely used machine learning paradigms for tabular data classification: gradient-boosted decision trees and deep neural networks.


## Installation
### TODO


## Usage
### On lxplus
The preprocessing part has to be done on the lxplus server since the root ntuples are too large to be copied. The command
```python
python preprocess_rdf.py
```
runs the script that produces preprocessed data suitable for the training of the generator and classifier. To produce a dataset with combined signal masses one can use
```python
python dataset_combine.py
```
command.
## On private machine
### TODO

