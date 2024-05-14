# eR2gm

This file contains information for the R pacakge 'eR2gm'. The package contains functions that calculate common psuedo R-squared statistics for exponential random graph models that include:

1) Efron's R-squared
2) McFadden's R-squared
3) Tjur's R-squared
4) Snidjer & Bosker's R-squared, called the "total variance" method
5) Cohen's R-squared
6) Cox-Snell R-squared

The functions adjust for the endogeneity of the model parameters. To do so, the functions calculate the change in psuedo R-squared from the full model, which includes endogeneous and exogeneous terms, and the model that only contains endogenous terms (e.g., GWDEGREE, GWDSP, GWESP, etc.).

NOTE: The user needs to specify the models correctly and ensure that they adjust for all the endogenous terms from their full model.


I choose the collection of different R-squared measures for different reasons:
- Efron's R-squared is most similar to R-squared for ordinary least squares "on paper" 
- Paul Allison demonstrates McFadden's and Tjur's R-squared statictics outperform other pseduo R-squared measures*
- the different measures sufficiently differ formulaically

* see Paul Allison's comparison of pseudo R-squared measures: https://statisticalhorizons.com/r2logistic/
