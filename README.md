# smart-meters-investigation
Interested in electricy demand and supply. Domestic smart meters should provide greater opportunity to understand demand side

Follow CRISP-DM (cross industry standard process for data mining)

# 1 - Business Understanding
- Pose at least three questions related to business or real-world applications of how the data could be used;
1. From selected data, how well can we predict electricity usage?
2. What parameters correlate with electricity usage?
3. What household characteristics demonstrate high and low usage?

# 2 - Data Understanding
Smart meter data and supporting infrmation from Kaggle dataset;
https://www.kaggle.com/jeanmidev/smart-meters-in-london

high dataset usability category

# 3 - Data Preparation
For size and processing time purpose, read in first data block sets to understand further.

From understanding the data, taking following approach;

merge daily household energy consumption with household information.

try use acron variables to predict energy consumption

data prep for supervised ML model;
map household category data (Acorn_grouped) to quant variable
https://chrisalbon.com/code/machine_learning/preprocessing_structured_data/encoding_ordinal_categorical_features/

# 4 - Modelling
supervised machine learning process:
fit model to training data to predict daily energy usage

# 5 - Evaluation
1. From selected data, how well can we predict electricity usage? A: Not well. More variables are needed to model.

![Screenshot 2021-10-29 at 15 53 25](https://user-images.githubusercontent.com/82510260/139456810-af5c53f7-754f-4c24-bcaf-bf21864e229e.png)

The total energy usage for the day correlates well with maximum half hour energy usage in that day, but that is not telling us much for predicting electicity usage. More variables are needed to model.

2. What parameters correlate with electircity usage? The household categorisation data (Acorn) does not correlate well.

![Screenshot 2021-10-29 at 15 51 00](https://user-images.githubusercontent.com/82510260/139456837-cb9ab06a-151c-4932-b771-bf64629e5ecd.png)


The household categorisation data (Acorn) does not correlate well. See coefs_df dataframe analysis at end of section 4 above - modelling. This Acorn coefficient has a low coefficient (0.11) with the linear model to predict total daily energy usage (daily_sum) for a household.

3. What household characteristics demonstrate high and low usage? Cannot tell from this model. More analysis and modelling needed.

where would take analysis next; time series analysis and include time series data (e.g. weather data), to try predict usage

# 6 - Deployment
Medium post: https://medium.com/@Phaedrus44/can-domestic-electricity-smart-meters-provide-greater-opportunity-to-understand-electricity-demand-625b7be23b53


# Acknowledgements
Took some ideas from following notebooks;
https://www.kaggle.com/tomneeld/dashboards-and-clustering
https://www.kaggle.com/rheajgurung/energy-consumption-forecast


# Installs / Pachages;


![Screenshot 2021-10-29 at 15 59 35](https://user-images.githubusercontent.com/82510260/139457735-87b2d91b-053b-4920-97d1-e1f0465850e3.png)
