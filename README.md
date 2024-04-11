# endocrine-disruption-explainer

<img src="TOC_4.jpeg" alt="drawing" width="200"/>

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.10963050.svg)](https://doi.org/10.5281/zenodo.10963050)

Endocrine Disruption Explainer is a code to generate structural alerts using Local Interpretable Model-Agnostic Explanations (LIME) of machine learning models from the TOX21, EDC and EDKB-FDA datasets.

The Endocrine Disruption Explainer framework is highly versatile (coded in Google Colab), with options that can be further developed and optimized by the users: it can accept any user-defined datasets (or datasets available in any repository), can use different fingerprints, data splitters, cross-validation methods, and any classification model from DeepChem or scikitlearn library.

There are ten codes that build the model using the curated and resampled TOX-21 dataset (5-fold cross-validated) with Rain Forest classifier and analyze the curated EDC or EDKB-FDA datasets:
1) tox21_AR_Resampling_EDC.ipynb explains the substructures important to the EDC dataset;
2) tox21_AR_Resampling_EDKB.ipynb explains the substructures important to the EDK-FDA dataset;
3) tox21_ER_Resampling_EDC.ipynb explains the substructures important to the EDC dataset;
4) tox21_ER_Resampling_EDKB.ipynb explains the substructures important to the EDKB-FDA dataset;
5) tox21_AhR_Resampling_EDC.ipynb explains the substructures important to the EDC dataset;
6) tox21_AhR_Resampling_EDKB.ipynb explains the substructures important to the EDKB-FDA dataset;
7) tox21_ARO_Resampling_EDC.ipynb explains the substructures important to the EDC dataset;
8) tox21_ARO_Resampling_EDKB.ipynb explains the substructures important to the EDKB-FDA dataset;
9) tox21_PPAR_Resampling_EDC.ipynb explains the substructures important to the EDC dataset;
10) tox21_PPAR_Resampling_EDKB.ipynb explains the substructures important to the EDKB-FDA dataset.

The original and curated TOX-21, EDC and EDKB datasets are provided here. DeepChem tools may also be used to upload any dataset in MoleculeNet or user-defined dataset. However, the TOX-21, EDC and EDKB-FDA datasets were curated removing duplicate and triplicate compounds, unifying compounds with two lables, and fixing smiles with RDKit issues. The TOX-21, EDC, and EDKB-FDA datasets were cross-validated to get the most robust models.

Endocrine Disruption Explainer was used with the Random Forest classifier, but any scikitlearn or DeepChem classifier may be used with little modification in the source code. And, these models were analyzed with different metrics (precision, accuracy, recall, MCC, and F1 scores) and with the confusion matrix. The models were optimized using hyperparameterization approach to get the best hyper parameters from each model and output the best results.

# Installation instructions

Endocrine Disruption Explainer is 100% compatible with Google Colab platform developed in Microsoft Windows using Python version 3.10.

Endocrine Disruption Explainer has the following dependencies: Lime, RDkit, DeepChem, Pandas, Matplotlib, sklearn, mols2grid, IPython and XlsxWriter.

# Documentation

The complete documentation about how to run the Endocrine Disruption Explainer protocol and several tutorials is being developed.

# Get help

The Endocrine Disruption Explainer is being actively developed and some issues may arise or you may need extra help to run Endocrine Disruption Explainer. In those cases, there are two main ways to get help:

1) Open a new issue in this repository
Or 
2) write an email to André Silva Pimentel (a_pimentel@puc-rio.br) (I will do my best to answer your questions as soon as possible).

# License

Endocrine Disruption Explainer is available under MIT License. See license document for more details. URL and DOI: https://github.com/andresilvapimentel/endocrine-disruptor-explainer (https://doi.org/10.5281/zenodo.10963050)

# Contributors

This code was written under collaboration:
Lucca Caiaffa Santos Rosa (Undergraduate student), Mariam Sarhan (Undergraduate student), and Andre Silva Pimentel (supervisor).
