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

Took some ideas from following notebooks;

https://www.kaggle.com/tomneeld/dashboards-and-clustering

https://www.kaggle.com/rheajgurung/energy-consumption-forecast

From understanding the data, taking following approach;

merge daily household energy consumption with household information.

try use acron variables to predict energy consumption

data prep for supervised ML model;
map household category data (Acorn_grouped) to quant variable
https://chrisalbon.com/code/machine_learning/preprocessing_structured_data/encoding_ordinal_categorical_features/

# 4 - Modelling
supervised machine learning process:
fit model to training data to predict daily energy usage

5 - Evaluation
1. From selected data, how well can we predict electricity usage? A: Not well. More variables are needed to model.
2. What parameters correlate with electircity usage? The household categorisation data (Acorn) does not correlate well.
3. What household characteristics demonstrate high and low usage? Cannot tell from this model. More analysis and modelling needed.

where would take analysis next;

time series analysis and include time series data (e.g. weather data), to try predict usage

# 6 - Deployment
Medium post: https://medium.com/@Phaedrus44/can-domestic-electricity-smart-meters-provide-greater-opportunity-to-understand-electricity-demand-625b7be23b53
