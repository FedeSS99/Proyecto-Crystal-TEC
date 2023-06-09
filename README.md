# Proyect-Crystal-TEC

## Description
The project had in foucs the analysis and modelling of social and economical parametes from 1990, whice have origin from USA census and additional crimininal information given by the FBI in 1995. The source of these datasets is located at the _Machine Learning_ repository of the _Center for Machine Learning and Intelligent Systems_ of University of California.

## Data information
The datasets can be found with the name of _Communities and Crime Data_ under the _Social_ tag and has the following characteristics:

- The data is multivariate and real.
- There is 1994 instances available, which represents the total communities in the study and 128 attributes to describe each instance.
- Some instances does not have all the attributes available.
- All the numerical attributes were normalized by a scale from 0 to 1.

## Objective
The objective attribute of name _ViolentCrimesPerPop_ represents the number of violent crimes per 100k habitants; which will be predicted by different regression techniques.

## Modelling
Three differente models were used to predict the goal variable with training and testing samples of 70% and 30%, respectively.

- Linear regression
- Decision Tree
- Random Forest

For the linear model, the coefficients were all considered as positive and no constant involved to prevent any negative predicted values. For the other models, hyper parameters were adjusted to find the optimal configuration that maximizes the R<sup>2</sup> constant.

## Results
The results for each model are shown in the Predicted vs Original values figures, along with a table that shows the Mean Squared Error, the Mean Absolute Error and the R<sup>2</sup> constant.

| Model | MS2 | MA | R2 |
| --- | --- | --- | --- |
| Linear | 0.0460 | 0.0347 | 0.5723 |
| Decision Tree | 0.0479 | 0.0345 | 0.5373 |
| Random Forest | 0.0428 | 0.0317 | 0.6395 |


<img src="./Resultados/ActualPredicho_LR.png" width="50%">
<img src="./Resultados/ActualPredicho_DT.png" width="50%">
<img src="./Resultados/ActualPredicho_RF.png" width="50%">
