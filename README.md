# IBM Data Science Capstone Project on SpaceX

## Overview

### Context
SpaceX has revolutionized the space industry with its commitment to making space exploration accessible to a broader audience. Its achievements include delivering payloads to the International Space Station, deploying a global internet satellite network, and conducting crewed space missions. A key to SpaceX's cost-efficiency is its groundbreaking ability to reuse the Falcon 9 rocket's first stage, which drastically reduces launch costs to $62 million compared to the $165 million average of competitors who cannot reuse their rockets. The feasibility of first-stage recovery is pivotal in determining launch costs, and through the analysis of publicly available data and the application of machine learning techniques, it is possible to forecast the likelihood of first-stage reuse for SpaceX and its rivals.

### Investigation Aims
- Examine how factors such as payload mass, launch site, flight frequency, and orbital paths influence the success of first-stage landings.
- Track the evolution of landing success rates over time.
- Identify the most effective prediction model for successful landings, focusing on binary outcomes.

### Summary of Findings
This study seeks to uncover the determinants of successful rocket landings using various analytical approaches:
- Data was gathered through the SpaceX REST API and web scraping.
- Data preparation involved creating a binary outcome variable to distinguish between successful and failed landings.
- Data exploration was conducted using visualization tools to assess the impact of payload size, launch location, flight count, and time trends.
- Data analysis was performed using SQL to derive statistics such as total and successful payload weights and launch outcomes.
- An examination of launch sites' success rates and their geographical positioning was conducted.
- Visual representations were created to highlight successful launch sites and payload categories.
- Predictive models were developed to forecast landing outcomes, employing techniques such as logistic regression, support vector machines (SVM), decision trees, and K-nearest neighbors (KNN).

### Key Insights from the Analysis:
- Progressive improvement in landing success rates was observed over time.
- Launch site KSC LC-39A demonstrated the highest success rate.
- Orbital paths ES-L1, GEO, HEO, and SSO achieved a 100% success rate.

### Visualization and Predictive Analysis:
- Launch sites are predominantly located near the equator and coastlines.
- The predictive models showed comparable performance, with the decision tree model marginally outperforming others in terms of the best score.

### Methodological Approach
#### Data Acquisition through API:
Data on rocket launches was retrieved from the SpaceX API, processed into a usable format, and converted into a DataFrame for analysis.

#### Web Scraping for Data Collection:
Falcon 9 launch data was extracted from Wikipedia, processed, and structured into a DataFrame for further analysis.

#### Data Preparation:
Launch outcomes were coded as binary values to distinguish between successful and unsuccessful landings.

#### Exploratory Data Analysis (EDA):
Graphical representations were employed to explore correlations and compare different factors.

#### Geographical Visualization:
Launch sites and outcomes were mapped to examine geographical influences on success rates.

#### Predictive Modelling:
Data was prepared and standardized for model training.
Various algorithms were tested to identify the most accurate predictive model.

### Conclusive Insights
- The decision tree model slightly surpassed others in performance on the test data.
- Launch sites near the equator benefit from the Earth's rotational speed, aiding in fuel and booster efficiency.
- Coastal launch sites facilitate operations and safety measures.
- An upward trend in launch success rates was noted.
- Launch site KSC LC-39A boasted the highest success rate, particularly for payloads under 5,500 kg.
- Orbits ES-L1, GEO, HEO, and SSO recorded a 100% success rate.
- Higher payload masses correlated with increased success rates across launch sites.

### Future Considerations
- A more extensive dataset could enhance the robustness of predictive analytics.
- Further feature analysis or principal component analysis (PCA) might improve model accuracy.
- Exploring the potential of advanced models like XGBoost could offer insights into its comparative effectiveness against other classifiers.
