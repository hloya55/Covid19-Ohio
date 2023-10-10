# Covid-19-in-Ohio README

## Overview
The dataset contains measurements on the level of awareness about Covid-19-related topics across all counties in Ohio during the pandemic. It includes the number of Covid-19 cases, deaths by county, and various county-level social, economic, and demographic variables. Each data point represents the level of awareness on specific issues for a particular day during the pandemic.

## Data Description
- **Period**: Starting from November 2019
- **Training Data**: 30% of all observations (3,141 observations)
- **Test Data**: 70% of all observations (7,331 observations)

## Data Collection
Awareness data has been extracted from tweets posted by users in Ohio during the Covid-19 pandemic. The dataset was prepared from over 46 million tweets posted by over 91,000 users. The process involved:
1. Collecting tweets from users in Ohio during the initial months of the pandemic.
2. Extracting co-occurring hashtags from these tweets to identify Covid-19 related topics.
3. Using similarity measures (Jaccard, Cosine, Intersection) to detect the intensity of discussions on these topics.

## Key Columns:
- `index`: Index associated with the observation
- `county`: Name of the Ohio county
- `cases`: Number of Covid-19 cases on a given day in a county
... [and many more]

## Awareness Topics:
The dataset measures awareness on various topics such as general Covid-19 awareness, domestic issues, economy, education, entertainment, foreign issues, gender, health, ideology, illness, nationalism, politics, race, religion, social issues, and sports. Awareness has been measured using different similarity measures like cosine, intersection, and Jaccard.

## Project Objectives:

### Part I: Descriptive Analysis
1. Summarize Ohio's Covid-19 experience.
2. Analyze average values for all topic awareness variables.
3. Investigate the `core_jaccard_normalized` variable.
4. Create county-level maps of Ohio showing average Covid-19 cases and deaths per capita.
5. Calculate average normalized Jaccard awareness scores for every day.

### Part II: Model Creation and Prediction
1. Train a model to predict the number of cases based on the dataset variables.
2. Report the R2-Value of the best model.
3. Participate in the Kaggle competition.
