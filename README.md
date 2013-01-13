imputation
==========

Missing data imputation (also known as matrix completion) is an extremely difficult science that tries
to fill in missing values of a dataset with the best guess.  Recently, it was popularized by the Netflix Challenge,
where a matrix of Netflix users and their movie ratings were presented to the data science community to see
if algorithms could be developed to predict how a user would rate a certain movie that the user has not yet seen.

##Imputation Algorithms Presented

* Mean Imputation
* k-Nearest Neighbors 
* SVD Imputation
* Robust SVD Imputation
* SVT Imputation
* Boosted Trees Imputation
* Persistence

##Algorithm Design
Each function in this package includes the imputation algorithm as well as a cross validatiion algorithm.  The CV
algorithm artificially eliminates 1/3 of the data in a dataset, and runs the imputation function.  Using the completed
data, the RMSE is calculated on the portion of the data that was artificially removed only.  Different imputation
algorithms will perform differently on different datasets, so it is important to have these functions for comparison.
