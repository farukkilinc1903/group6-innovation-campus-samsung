
# Model Exploration & Results

# 1) Model Choice & Justification
In this study, the Random Forest Regressor was selected as the primary predictive model to analyze the factors influencing electricity access in schools. The choice of this model is based on several key advantages.
First, the relationship between socio-economic indicators (such as GDP, urbanization, and inequality) and infrastructure outcomes is inherently non-linear, making linear models insufficient for capturing complex patterns. Random Forest, as an ensemble learning method, effectively models these non-linear relationships.
Second, the model is robust to outliers and noise, which are common in global datasets derived from multiple sources. This improves the reliability of predictions across diverse country-level data.
Finally, Random Forest provides a feature importance mechanism, allowing the identification and quantification of the most influential variables affecting electricity access in schools. This capability is essential for interpreting the model in the context of sustainable development

# 2) Data Preparation
The dataset used in this analysis was constructed by integrating multiple data sources, including NASA SEDAC indicators, World Bank datasets, and school electricity access data.
To ensure consistency, all datasets were merged using ISO country codes and year as common identifiers. World Bank datasets, originally in wide format, were transformed into a long (panel) format using a melting process, enabling time-series analysis across countries.
Key preprocessing steps included:
•	Filtering relevant years and variables 
•	Renaming columns for clarity and consistency 
•	Merging datasets into a unified structure 
•	Handling missing values by removing incomplete observations 
After preprocessing, the final dataset was structured as a clean panel dataset suitable for machine learning analysis.
To evaluate model performance, the dataset was split into 80% training data and 20% testing data, ensuring that the model was assessed on unseen observations.

# 3) Training & Evaluation
The Random Forest model was trained on the prepared dataset to predict electricity access in schools based on socio-economic and infrastructure indicators.
Model performance was evaluated using the coefficient of determination (R²), which measures how well the independent variables explain the variance in the target variable.
The model achieved an R² score of 0.916, indicating that approximately 91.6% of the variability in school electricity access is explained by the model. This represents a strong predictive performance and suggests that the selected variables capture the underlying patterns effectively.
Feature importance analysis further revealed that national electricity access, urban population, and GDP per capita are among the most influential predictors, while variables such as education expenditure have comparatively lower explanatory power.
These results highlight the critical role of overall energy infrastructure and economic development in determining electricity access in schools.
•	National electricity access is the most significant predictor, highlighting that school-level access is largely dependent on overall national energy infrastructure. 
•	Urban population percentage and GDP per capita also play substantial roles, reflecting the importance of economic development and urbanization in infrastructure distribution. 
•	Income inequality (Gini index) shows a negative relationship, suggesting that higher inequality is associated with lower electricity access in schools. 
•	Notably, education expenditure was found to be less influential than expected, indicating that financial investment alone is insufficient without supporting infrastructure. 
One of the most distinctive findings of this study is the role of NASA-derived light per capita (Lpc), a satellite-based proxy for economic activity and infrastructure. This variable demonstrated stronger explanatory power than education expenditure, emphasizing the value of remote sensing data in development analysis.

# 4) Interpretation in the Context of SDGs
The findings clearly demonstrate that achieving SDG 4 (Quality Education) is closely linked to progress in SDG 7 (Energy Access). Investments in education must be complemented by improvements in national energy infrastructure to be effective. Without reliable electricity, educational resources cannot be fully utilized, regardless of financial spending.

# 5) Limitations & Future Improvements
This study has several limitations. First, the analysis is restricted to the period 1992–2013 due to the availability of NASA data, which may limit the representation of recent trends. Second, missing data in variables such as education expenditure reduced the number of countries included in the analysis, potentially affecting generalizability.
Future research could address these limitations by incorporating more recent VIIRS satellite data and expanding the analysis to sub-national levels, such as regions or cities, to capture more localized patterns of inequality.




# Exploratory data analysis

# 1) Project Name 

Exploring Global Electricity Access in Schools Through Data Visualization to Support SDG 4 and SDG 7 

# 2) Overview 

This project explores global electricity access in schools using data visualization techniques to support Sustainable Development Goal 4 (Quality Education) and Sustainable Development Goal 7 (Affordable and Clean Energy). Electricity access in schools plays a crucial role in improving educational quality by enabling digital learning tools, lighting, internet connectivity, and modern teaching methods. 

The primary objective of this project is to analyze the relationship between school electricity access and several socio-economic indicators such as; 
GDP per capita,  
national electricity access,  
urban population,  
education expenditure.  
By visualizing these relationships, we aim to identify global patterns and inequalities in electricity access across different countries. 

Through exploratory data analysis (EDA) and visualizations such as scatter plots, histograms, and correlation of heatmaps, the project highlights trends that may help policymakers understand the factors influencing electricity availability in schools. These insights can support strategies aimed at improving energy infrastructure in educational environments. 

Ultimately, this project demonstrates how data analysis can contribute to sustainable development by revealing key relationships between energy access and educational opportunities worldwide. 

# 3) Background 

Access to electricity is a fundamental requirement for modern education systems. Schools with reliable electricity can utilize computers, projectors, internet access, and digital learning platforms, significantly enhancing teaching and learning experiences. However, many schools in developing countries still lack consistent electricity access, limiting educational opportunities and widening global inequalities. 

According to international development reports, the lack of electricity in schools often correlates with broader infrastructure challenges such as limited national electricity coverage, lower economic development, and rural isolation. Understanding these relationships is essential for addressing educational inequalities and promoting sustainable development. 

Data-driven approaches provide an effective way to analyze such global challenges. By combining datasets related to electricity access, economic indicators, and demographic factors, researchers can identify patterns and relationships that may not be immediately visible. 

This project focuses on using data visualization and exploratory data analysis to better understand how electricity access in schools relates to national economic and infrastructure indicators. The findings may provide useful insights for improving both educational outcomes and energy accessibility. 

# 4) Key Objectives / Business Objectives 

a) Research Questions 

What is the global distribution of electricity access in schools? 

Is there a relationship between national electricity access and electricity access in schools? 

How does GDP per capita influence electricity availability in schools? 

Does urbanization play a role in improving electricity access in educational institutions? 

Is there a relationship between education expenditure and school electricity access? 

Which socio-economic indicator has the strongest correlation with electricity access in schools? 

 

b) Key Steps 

Collect and combine datasets related to electricity access in schools and relevant socio-economic indicators. 

Clean and preprocess the data to remove missing or inconsistent values. 

Perform exploratory data analysis (EDA) to understand the dataset structure. 

Calculate descriptive statistics to summarize the data. 

Visualize relationships between variables using charts and plots. 

Identify patterns and correlations between school electricity access and other indicators. 

Interpret results and discuss their implications for sustainable development goals. 

 

# 5) Methods and Workflow 

a) Datasets 

The project uses multiple publicly available datasets related to global development indicators, including: 
Electricity access in schools dataset 
GDP per capita data 
Urban population statistics 
National electricity access rates 
Education expenditure indicators 
These datasets are combined to analyze relationships between electricity infrastructure and educational access. 

 

b) Data Cleaning and Preprocessing 

The preprocessing stage includes several steps to prepare the dataset for analysis: 
Filtering the dataset for relevant years and countries. 
Renaming columns for clarity and consistency. 
Merging multiple datasets based on country identifiers. 
Identifying and handling missing values. 
Removing incomplete observations to ensure reliable analysis. 

 

c) Exploratory Data Analysis (EDA) 

The exploratory analysis includes: 
Descriptive statistics to summarize the dataset. 
Histograms to understand the distribution of variables. 
Correlation heatmaps to identify relationships between indicators. 
Scatter plots to visualize relationships between variables such as: 
GDP per capita vs school electricity access 
National electricity access vs school electricity access 
Urban population vs school electricity access 
These visualizations help identify key trends and patterns within the data. 

 

d) Deliverables 

A comprehensive exploratory data analysis of global electricity access in schools. 
Data visualizations illustrating relationships between electricity access and socio-economic indicators. 
Insights highlighting factors that influence electricity availability in schools. 
A project report summarizing methodology, analysis, and findings. 
Presentation materials explaining the project and its contribution to SDG 4 and SDG 7. #
