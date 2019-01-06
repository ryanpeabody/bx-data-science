# lending-club-analysis
Exploration, analysis, and modeling of Lending Club loan origination data

## Part 1: Exploratory Data Analysis
Most features adhere to roughly Gaussian distributions, with varying degrees of skew. Most variance in the system can be explained by variations in loan amounts and interest rates, which suggest some minor separation between loan grades associated with these modes of variation. In general, Lending Club's interest rates and loan amounts have increased, as well as the average debt that it's lendees carry before they borrow. These trends are exacerbated among lendees with riskier profiles.

## Part 2: Busines Analysis
1. 83.54% of 36-month loans have been fully paid
2. 35/35 (100%) 2007 G grade 36-month loans defaulted
3. Including loans that have been paid, as well as loans that have defaulted, 36-month loans generated an ARR of 0.000915

## Part 3: Modeling
A logistic regressor does a poor job of modeling defaults. The area under the ROC curve, as well as simple accuracy, and evaluations of the number of defaults and non-defaults that were falsely predicted by the model suggest that it is inaccurate, and would result in worse financial outcomes than Lending Club's current approach. Either more features should be used, a non-linear classifier should be used, and/or the regressor's cost function should be adjusted to penalize allowing a loan that results in default more heavily in order to minimize risk and loss of money.
