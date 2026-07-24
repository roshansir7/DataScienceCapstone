Winning the Space Race with Data Science
Project Overview

This data science capstone project analyses SpaceX Falcon 9 launch data and develops machine-learning models to predict whether the rocket’s first stage will land successfully.

The ability to reuse the first stage significantly reduces launch costs. Therefore, predicting landing success can provide valuable information to organisations evaluating launch performance, operating conditions and potential competition with SpaceX.

Project Objectives
Collect Falcon 9 launch data from the SpaceX REST API.
Scrape historical Falcon 9 launch records from Wikipedia.
Clean, transform and prepare the collected data.
Explore factors affecting landing success using Python visualisations and SQL.
Analyse launch-site locations using interactive Folium maps.
Build an interactive Plotly Dash dashboard.
Train and evaluate classification models to predict landing success.
Project Workflow
1. Data Collection

Launch information was collected from the SpaceX API using Python Requests. Additional historical launch records were extracted from Wikipedia using BeautifulSoup and converted into Pandas DataFrames.

2. Data Wrangling and Feature Engineering

The datasets were cleaned and prepared by:

Handling missing values.
Selecting Falcon 9 launch records.
Creating a binary landing-success label.
Encoding categorical variables.
Standardising numerical features.
Preparing training and testing datasets.
3. Exploratory Data Analysis

Exploratory analysis was completed using Pandas, Matplotlib, Seaborn and SQL. The analysis examined relationships between landing success and:

Launch site
Payload mass
Orbit type
Flight number
Booster version
Launch year
4. Interactive Visual Analytics

Folium was used to map launch sites and their proximity to coastlines, roads, railways and populated areas.

A Plotly Dash application was also developed with:

A launch-site selection dropdown.
Success and failure pie charts.
A payload-range slider.
Interactive payload-versus-landing-outcome scatter plots.
5. Machine-Learning Prediction

The following classification algorithms were trained and compared:

Logistic Regression
Support Vector Machine
Decision Tree
K-Nearest Neighbours

GridSearchCV was used for hyperparameter tuning, while accuracy and confusion matrices were used to evaluate model performance.

Key Findings
Landing success generally increased as SpaceX gained more launch experience.
KSC LC-39A demonstrated strong launch-success performance.
Launch site, orbit type, payload mass and flight history influenced landing outcomes.
SpaceX launch sites were located close to coastlines and transport infrastructure.
The Decision Tree classifier produced the strongest performance among the evaluated models.
False-positive predictions remained the main classification challenge.
Technologies Used
Python
Pandas and NumPy
Requests and BeautifulSoup
SQL and Db2
Matplotlib and Seaborn
Folium
Plotly and Dash
Scikit-learn
Jupyter Notebook
Repository Contents

The repository contains notebooks and code for:

SpaceX API data collection
Wikipedia web scraping
Data wrangling
Exploratory data analysis
SQL analysis
Folium map visualisation
Plotly Dash dashboard development
Machine-learning prediction
