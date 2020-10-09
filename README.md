# synthetic_data_pilot


[![DOI](https://zenodo.org/badge/302670560.svg)](https://zenodo.org/badge/latestdoi/302670560)

This repository is being updated as research is performed. The experiments (and required data) are available as Jupyter Notebooks.

For any queries on this work contact m.allen@exeter.ac.uk


## Set up environments locally

These notebooks require a range of environments, depending on the method. Please see instructions in environment_yamls directory.

Environment names (these may be changed in the yaml files):

* synthetic_pytorch (for GAN)
* synthetic_tensorflow (for VAE)
* smote (for SMOTE)
* ctgan (for CTGAN)

The PCA-based method may be run using any environment

## Aim

To test the utility of a range of data synthesis techniques for use in machine learning, especially focussed on clinical data sets.

## Problem

Patient-level health data is sensitive information and is often not suitable to be shared with machine learning models trained using that data. How can we share patient-level data so that machine learning models may be tested/improved?

## Suggested solution

Use data synthesis techniques to create a synthetic data set that behaves like real patient data, and an be used to train and test machine learning models.

## Techniques to test:

* PCA (Principal Component Analysis)
* SMOTE (Synthetic Minority Oversampling Technique)
* GANs (Generative Adversarial Networks)
* VAEs (Variational AutoEncoders)

As an alternative to synthetic data we will also examine the use of differential provacy techniques.

## Health data sets to test

Used:

* https://www.kaggle.com/uciml/breast-cancer-wisconsin-data
* https://raw.githubusercontent.com/MichaelAllen1966/1807_stroke_pathway/master/machine_learning/data/data_for_ml_clin_only.csv

Others:

* https://www.kaggle.com/ronitf/heart-disease-uci
* https://www.kaggle.com/uciml/pima-indians-diabetes-database
* https://www.kaggle.com/joniarroba/noshowappointments
* https://www.kaggle.com/loveall/cervical-cancer-risk-classification
* https://www.kaggle.com/sammy123/lower-back-pain-symptoms-dataset
* https://www.kaggle.com/uciml/indian-liver-patient-records
