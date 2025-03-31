# Ergonomics
Statistical Modelling For Ergonomics 

First coding project without prior knowledge. Although use my own ability to create regression paraemeters, used Claude to vibe code the design.

Important step, Formulate the best MLR equation. This will be based on the NYC Compensation data from Kaggle

https://www.kaggle.com/datasets/thedevastator/workers-compensation-claims-in-new-york-state-20 This data set uses Work Incentive Benefits Councelling in comparsion to taught WSIB

1. First removed 390k data from 0$ income inputs, a filter. 100k data points took too long to compile.
2. Apply ridge regression to address multicollinearity. Variables are very closely correlated to each other, we must address this issue to get more precise estimatees of the regression coefficients. Ridge regressions because parameteres are highly correlated. By using this mdoel I could address coliniearity by adding a hyperparameter labmda. L2 penalty that shrinks coefficients towards zero but never to abosulte zero. Good for machine learning models.
3. Next found the best model for MLR based on a subset.
4. Choose three predictors: Average Salary, Replacement Worker Cost, and NEER Extra Injury Cost
5. Clean data and convert to numeric format.
6. Handle missing values using median imputation. 
7. Standardize variables for numerical stability.
8. Convert coefficients back to original scale
9. Interpret coefficients to understand cost drivers.
10. Model in a simple 2D regression plane. However this does not address the fixed NEER cost, thus 3d is preffered.
11. Implemented 3D mesh graph with regression/plane with calculations and error terms. Very good model, fits very well.

