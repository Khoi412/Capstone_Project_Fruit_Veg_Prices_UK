# ![CI logo](https://codeinstitute.s3.amazonaws.com/fullstack/ci_logo_small.png)

# Project Summary 

- Fruit & Veg Prices in the UK (2017-2022)
- The UK's Horticulture sector saw it's home-produced vegetables value grow from approx £1.5 Billion in 2017 to £1.8 Billion in 2022 and it's fruits produce from £920 Million in 2021 to £1,046 Billion in 2022. 

# Dataset Content

- Data is source from Kaggle https://www.kaggle.com/datasets/datota/fruit-and-vegatable-prices-in-uk-2017-2022

- Total entries: 9,647 rows and 6 columns

- Timeframe: 2017–2022

- Dataset includes information about fruit and veg, what type and pricing over a 5 year period


|           | category           | item        | variety          | date         | price      | unit | 
|-----------|--------------------|-------------|------------------|--------------|------------|------|
|0          | fruit              |      apples |bramleys_seedling |2022-03-11    |  2.05      |  kg  |
|1          | fruit              |      apples |coxs_orange_group |2022-03-11    |  1.22      |  kg  |
|2          | fruit              |      apples |  egremont_russet |2022-03-11    |  1.14      |  kg  |
|3          | fruit              |      apples |         braeburn |2022-03-11    |  1.05      |  kg  |
|4          | fruit              |      apples |             gala |2022-03-11    |  1.03      |  kg  |
|...        |   ...              |         ... |              ... |       ...    |   ...      | ...  |
|9642       | cut_flowers        | alstromeria |           indoor |2017-11-03    |  0.27      | stem |
|9643       | cut_flowers        |chrysanthemum|     indoor_spray |2017-11-03    |  0.22      | stem |
|9644       | cut_flowers        |      lillies|         oriental |2017-11-03    |  0.70      | stem |
|9645       | cut_flowers        |    narcissus|           indoor |2017-11-03    |  0.06      | stem |
|9646       | pot_plants         |     cyclamen|            13_cm |2017-11-03    |  0.75      | unit |

[9647 rows x 6 columns]


# Buisness Requirements

- A fictional international business conglomerate has an interest in the fresh produce sector in the food industry business in the UK. The client has requested that a data analyst analyse the dataset of fruits and vegetable prices and determine:

1. To identify the optimal season to procure and sell fresh produce.

2. Monitor price volatility to inform purchasing and inventory decisions.

3. Compare variety-level pricing (e.g., types of apples).


# Hypotheses and Validation

- Hypothesis 1:
    - On-season produce is significantly cheaper than off-season
    - Validation: Compare mean prices grouped by Season.

- Hypothesis 2:
    - Off-season fruit and veg produce has a high volatile price
    - Validation: Use Standard deviation prices grouped by Season.

- Hypothesis 3:
    - Some varieties of the same fruit and veg are cheaper than it's other variants
    - Validation: Group by variety and compare mean and std pricing. 


# Summary on my findings with the Hypotheses and Business Requirements

- Apples offer stable year-round supply, with premium opportunities in unique or heritage varieties. Variety segmentation is useful for pricing strategy — e.g., marketing higher-margin varieties differently from commodity ones.

- Cabbages provide price stability, ideal for budgeting in food service or wholesale. Price competition is strong — differentiation must come from freshness, local sourcing, or packaging, not price alone.

- The price of strawberries shows a clear seasonal trend. On-season prices (May–Aug) are concentrated and lower, reflecting ample supply. Off-season (Jan–Mar, Oct–Dec) prices rise and become more variable, due to scarcity. Shoulder-season prices are the most unpredictable, sometimes spiking higher than any other season. This highlights the importance of seasonal planning in procurement and pricing strategies."


# Project Plan


# The rationale to map the business requirements to the Data Visualisations


# Analysis techniques used


# Ethical considerations


# Unfixed Bugs


# Development Roadmap


# Main Data Analysis Libraries


# Credits


# Content


# Media


# Acknowledgements (optional)


## Deployment Reminders

* Set the `.python-version` Python version to a [Heroku-22](https://devcenter.heroku.com/articles/python-support#supported-runtimes) stack currently supported version that closest matches what you used in this project.
* The project can be deployed to Heroku using the following steps.

1. Log in to Heroku and create an App
2. At the **Deploy** tab, select **GitHub** as the deployment method.
3. Select your repository name and click **Search**. Once it is found, click **Connect**.
4. Select the branch you want to deploy, then click **Deploy Branch**.
5. The deployment process should happen smoothly if all deployment files are fully functional. Click the button **Open App** at the top of the page to access your App.
6. If the slug size is too large, then add large files not required for the app to the `.slugignore` file.
