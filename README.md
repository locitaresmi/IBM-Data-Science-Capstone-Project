# **SpaceX Falcon 9 First Stage Landing Prediction**

## **Project Overview**
This project focuses on predicting the success of Falcon 9’s first stage landing. The success of these landings is crucial for reducing launch costs, as SpaceX reuses the first stage for subsequent missions, saving millions per launch. The project utilises historical data from SpaceX API and additional data from web scraping to build a predictive model for these landings. This analysis provides insights into the factors influencing landing success, such as booster version, payload mass, orbit, and launch site.

## **Key Features**
- **Data Collection**: Historical launch data was gathered from the SpaceX API and supplemented with data scraped from Wikipedia.
- **Data Wrangling**: Data cleaning and transformation processes were applied to ensure the dataset was ready for analysis. Key features like payload mass, landing outcome, and booster version were extracted.
- **EDA (Exploratory Data Analysis)**: Visualisations, including scatter plots, bar charts, and line charts, were used to explore the relationships between different variables.
- **SQL Queries**: SQL queries were utilised to perform detailed exploration of the dataset, focusing on payload mass, landing outcomes, and success rates at various launch sites.
- **Predictive Model**: A machine learning classification model was developed to predict the likelihood of a successful landing, using algorithms like Logistic Regression, K-Nearest Neighbours (KNN), Decision Tree, and Support Vector Machine (SVM).
- **Interactive Dashboard**: A Plotly Dash dashboard was built, allowing users to explore the success rates of launches based on different parameters such as launch site, payload range, and booster version.

## **Technologies Used**
- **Python**: For data processing, visualisation, and model building.
- **Plotly Dash**: For creating an interactive web-based dashboard.
- **Pandas**: For data manipulation and analysis.
- **SQLite**: For querying the dataset with SQL.
- **BeautifulSoup**: For web scraping launch records from Wikipedia.
- **Scikit-Learn**: For implementing machine learning models.

## **Data Collection**
- **SpaceX API**: Data on launches, payloads, and landing outcomes was collected using the SpaceX API.
- **Web Scraping**: Wikipedia pages containing historical launch records were scraped to enrich the dataset, filling in gaps from the API data.

## **Exploratory Data Analysis (EDA)**
- **Key Visualisations**:
  - **Flight Number vs. Payload Mass**: To understand the relationship between flight experience and payload mass, and how these factors affect landing success.
  - **Success Rate by Orbit Type**: To see how different orbital missions impact the likelihood of a successful landing.
  - **Payload Mass vs. Launch Site**: To investigate how payload mass varies by launch site and its effect on landing success.
  - **Launch Success Yearly Trend**: To track the improvement in landing success rates over time.

## **SQL Queries**
- Example queries:
  - **Total Payload Mass**: Calculate the total payload mass carried by NASA’s missions.
  - **First Successful Ground Landing Date**: Retrieve the date of the first successful ground landing.
  - **Launch Success by Site**: Display the success rate of launches at different sites.

## **Machine Learning Models**
The project utilised multiple machine learning algorithms to predict landing success, including:
- **Logistic Regression**
- **K-Nearest Neighbours (KNN)**
- **Decision Tree**
- **Support Vector Machine (SVM)**

Hyperparameter tuning was conducted using GridSearchCV for optimal performance, and the models were evaluated based on accuracy on the test dataset.

## **Interactive Dashboard**
The Plotly Dash dashboard includes:
- **Launch Site Dropdown**: Select a specific launch site or view data for all sites combined.
- **Payload Range Slider**: Filter launches based on payload mass.
- **Success Pie Chart**: Visualise the success rates of selected launches.
- **Success-Payload Scatter Plot**: Display the relationship between payload mass and launch outcome, with points coloured by booster version.

## **Contributors**
- **Author**: Wening Dyah Locitaresmi
- **Contributors**: Project guided by resources and example projects from IBM and Coursera.
