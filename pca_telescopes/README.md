# PCA - Classifying Particles
This project explores Principle Component Analysis (PCA) through classifying particles into gammes or hadrons. As the features are correlated, PCA will be necessary to get a new set of features, and select the features with the most information. 

This project is based on Codecademy's [PCA Project](https://www.codecademy.com/paths/fe-path-feature-engineering/tracks/fe-feature-engineering-reducing-dimensionality/modules/fe-principal-component-analysis-pca/projects/fe-pca-project). 

## Dataset
The dataset, `telescopes.csv` was generated as desrcibed in `D. Heck et al., CORSIKA, A Monte Carlo code to simulate extensive air showers, Forschungszentrum Karlsruhe FZKA 6019 (1998)`. 

## Methods
* Manual eigendecomposition
* PCA with 7 components
* PCA with 2 components
* PCA-SVC and no-PCA-SVC to classify particles

## Results and Significance
Testing score for PCA-SVC: 0.74
Testing score for non-PCA-SVC: 0.72

As can be seen from the testing scores of the 2 models, the PCA-SVC has a higher score than the non-PCA-SVC, showing that PCA is a strong feature engineering strategy for correlated features. 