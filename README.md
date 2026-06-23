**Falcon 9 First-Stage Landing Prediction**

**Applied Data Science Capstone Project**

**Executive Summary**

This project investigates the factors influencing the successful recovery of Falcon 9 first-stage boosters and develops machine learning models to predict landing outcomes. SpaceX has significantly reduced launch costs through reusable rocket technology, lowering launch expenses to approximately $62 million per mission compared to the industry average of around $165 million.

Using historical Falcon 9 launch data collected from the SpaceX API and publicly available sources, this project applies data analytics, geospatial visualization, interactive dashboards, and machine learning techniques to analyze launch performance and forecast booster landing success. The results demonstrate that historical mission characteristics contain meaningful patterns that can be leveraged to support launch cost estimation and reusability analysis.

**Project Background**

SpaceX has transformed the commercial space industry through the successful implementation of reusable rocket technology. The ability to recover and reuse Falcon 9 first-stage boosters has improved operational efficiency, increased launch frequency, and substantially reduced mission costs.

As a Data Scientist working for the fictional aerospace company Space Y, the objective of this project was to analyze historical Falcon 9 launch records and identify the factors that contribute to successful booster landings. By understanding these factors and developing predictive models, organizations can gain insights into launch economics, mission planning, and competitive positioning within the space industry.

**Project Objectives**

The project aims to answer the following key questions:

- Which launch sites contribute the most to successful launches and booster recoveries?
- How do payload mass, orbit type, and booster version influence landing success?
- What operational trends and patterns can be identified from historical Falcon 9 missions?
- Can machine learning models accurately predict first-stage landing outcomes?
- Which predictive model provides the most reliable performance for landing success prediction?

**Methodology**
**Data Collection**

Historical Falcon 9 launch records were collected from multiple sources. Launch data was retrieved through the SpaceX API, while supplementary mission information was obtained through web scraping of publicly available Wikipedia launch records. The collected data was integrated into a unified dataset for analysis.

**Data Wrangling and Preparation**

The dataset was cleaned and preprocessed to ensure consistency and quality. Missing values were handled, data formats were standardized, and additional features were created to support analysis and predictive modeling.

**Exploratory Data Analysis (EDA)**

Exploratory analysis was conducted using Python and SQL to identify relationships between launch variables and landing outcomes. Visualizations and statistical summaries were used to uncover trends involving payload mass, launch sites, booster versions, orbit types, and mission success rates.

**SQL Analysis**

The processed dataset was loaded into a Db2 database environment where SQL queries were used to investigate launch frequencies, payload statistics, mission outcomes, and booster performance across different launch locations.

**Geospatial Analysis**

Folium was used to create interactive maps visualizing launch site locations and nearby geographical features. Distance analysis examined proximity to coastlines, transportation infrastructure, and populated areas, highlighting the strategic positioning of launch facilities.

**Interactive Visual Analytics**

An interactive Plotly Dash application was developed to enable dynamic exploration of Falcon 9 launch data. Users can analyze launch success rates, payload distributions, and mission characteristics through interactive charts, filters, and visualizations.

**Machine Learning Modeling**

Several supervised machine learning algorithms were trained and evaluated to predict first-stage landing success:

- Logistic Regression
- Support Vector Machine (SVM)
- Decision Tree Classifier
- K-Nearest Neighbors (KNN)

GridSearchCV was used for hyperparameter optimization, and model performance was assessed using accuracy scores, confusion matrices, and test-set evaluation metrics.

**Tools and Technologies**

**Programming and Analysis**

- Python
- Pandas
- NumPy
- SQL
- IBM Db2

**Data Visualization**

- Matplotlib
- Seaborn
- Plotly Dash
- Folium

**Data Collection**

- SpaceX API
- BeautifulSoup
- Web Scraping

**Machine Learning**

- Scikit-learn
- Logistic Regression
- Support Vector Machine (SVM)
- Decision Tree
- K-Nearest Neighbors (KNN)
- GridSearchCV

**Results**
**Dataset Development**

A structured and analysis-ready Falcon 9 dataset was successfully created by integrating data from multiple sources and applying data cleaning and preprocessing techniques.

**Exploratory Analysis Findings**

The analysis revealed several important relationships between mission characteristics and landing outcomes:

- Launch site selection influences mission performance.
- Booster version impacts landing reliability.
- Orbit type affects recovery success rates.
- Successful missions occur across a wide range of payload masses.

**SQL Insights**

Database queries provided valuable insights into:

- Launch site activity
- Mission frequencies
- Payload distributions
- Booster utilization patterns
- Landing success trends
-
**Geospatial Findings**

Interactive Folium maps demonstrated that launch sites are strategically positioned near coastlines while maintaining safe distances from densely populated areas. Transportation infrastructure surrounding launch facilities further supports operational efficiency.

**Interactive Dashboard**

The Plotly Dash dashboard enables users to:

- Explore launch success rates by site
- Analyze payload mass distributions
- Investigate mission outcomes
- Compare launch performance across different mission parameters

**Machine Learning Performance**

Several classification algorithms were evaluated for landing outcome prediction
**Model and Test Accuracy:**

Logistic Regression : 83.3%
Support Vector Machine (SVM): 83.3%
Decision Tree Classifier : 83.3%
K-Nearest Neighbors (KNN): 83.3%

**Key Findings**
**High Launch Reliability**

Historical launch records demonstrate that SpaceX consistently achieves successful missions, reflecting strong operational reliability and engineering performance.

**Importance of Launch Sites**

KSC LC-39A and CCAFS LC-40 contributed the highest number of successful launches and booster recoveries, emphasizing the importance of launch infrastructure.

**Advancement of Reusable Rocket Technology**

Landing outcomes improved significantly over time, evolving from early failures and recovery attempts to frequent successful landings on both drone ships and landing pads.

**Payload Mass Is Not a Primary Limitation**

Successful booster recoveries occurred across both low and high payload ranges, suggesting that payload mass alone does not significantly reduce landing success.

**Improved Performance of Newer Boosters**

FT and Block-series Falcon 9 boosters demonstrated higher reliability and successfully supported larger payloads, highlighting ongoing technological advancements.

**Predictive Potential of Historical Data**

Historical launch characteristics provide sufficient information to predict landing outcomes with strong accuracy using machine learning techniques.

**Conclusion**

This project demonstrates the successful application of data science methodologies to a real-world aerospace problem. By combining data collection, data wrangling, SQL analysis, geospatial visualization, interactive dashboards, and machine learning, valuable insights were generated regarding Falcon 9 launch operations and booster recovery performance.

The findings indicate that launch site selection, booster generation, and mission characteristics play important roles in landing success. Furthermore, predictive models can effectively forecast booster recovery outcomes, supporting launch cost estimation and operational decision-making.

Future enhancements may include incorporating weather conditions, environmental factors, booster refurbishment history, and additional mission-specific variables to further improve model accuracy and predictive capabilities.

**Repository Structure**
data/
├── Raw and processed datasets

notebooks/
├── Data collection notebooks
├── Data wrangling notebooks
├── EDA notebooks
├── SQL analysis notebooks
├── Machine learning notebooks

dash_app/
├── Plotly Dash application files

reports/
├── Presentation slides
├── Final report
├── Visualizations

README.md

**Acknowledgments**

- IBM Data Science Professional Certificate
- Coursera
- SpaceX API
- Wikipedia Launch Records
- Open-source Python Data Science Community
