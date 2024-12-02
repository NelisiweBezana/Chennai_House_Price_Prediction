# Chennai Housing Sales Price Prediction

## Project Overview
This project involves analyzing and predicting the sales prices of residential properties in Chennai, India. The dataset used in this project contains detailed information about various properties, including their location, size, amenities, and sale details. The goal is to build a predictive model that can accurately estimate the sales prices of properties based on these attributes.

## Dataset

### Description
The dataset consists of 7,056 records and 22 fields, offering insights into different aspects of the properties. The dataset requires significant preprocessing and cleaning due to missing values, incorrect data, and outliers. The key features of the dataset include property characteristics like area, size, number of rooms, and sale price.

### Attributes
- **PRT_ID**: Unique identifier for each property.
- **AREA**: The locality where the property is situated.
- **INT_SQFT**: Internal square footage of the property.
- **DATE_SALE**: Date when the property was sold.
- **DIST_MAINROAD**: Distance from the property to the nearest main road.
- **N_BEDROOM**: Number of bedrooms.
- **N_BATHROOM**: Number of bathrooms.
- **N_ROOM**: Total number of rooms.
- **SALE_COND**: Condition under which the property was sold.
- **PARK_FACIL**: Availability of parking facilities.
- **DATE_BUILD**: The year the property was built.
- **BUILDTYPE**: Type of building (e.g., apartment, independent house).
- **UTILITY_AVAIL**: Availability of utilities (water, electricity, etc.).
- **STREET**: Type of street where the property is located.
- **MZZONE**: Municipal zone where the property is located.
- **QS_ROOMS**: Quality score of the rooms.
- **QS_BATHROOM**: Quality score of the bathrooms.
- **QS_BEDROOM**: Quality score of the bedrooms.
- **QS_OVERALL**: Overall quality score of the property.
- **REG_FEE**: Registration fee for the property.
- **COMMIS**: Commission amount for the sale.
- **SALES_PRICE**: The final sales price of the property (target variable).

## Exploratory Data Analysis (EDA)

### Purpose
The purpose of the exploratory data analysis (EDA) was to uncover patterns, trends, and relationships within the dataset. Through statistical analysis and visualizations, we aimed to understand the relationships between various features and how they influence the sales price of properties.

### Key Insights from EDA
- **PROP_SIZE** (internal square footage) showed strong correlations with the number of rooms, bedrooms, and bathrooms, as well as with the sales price.
- **SALES_PRICE** was strongly influenced by the **REG_FEE** (registration fee) and **QS_OVERALL** (overall quality score of the property).
- **DIST_MAINROAD** had no significant correlation with other features or the sales price.
- Certain areas, such as **Karapakam**, showed significant fluctuations in sales prices between 2010 and 2012.

### Visualizations
- Distribution of **SALES_PRICE** across the dataset.
- Correlation heatmap showing the relationships between numerical features.
- Distribution of properties across different **AREAs** and trends of **SALES_PRICE** over time.

## Data Preprocessing and Cleaning

### Missing Values and Outliers
The dataset contained missing values and outliers, which were handled by imputing missing values where appropriate and removing outliers that could skew the model results.

### Feature Engineering
New features were derived from existing attributes, such as extracting the year of sale from the **DATE_SALE** field to enable trend analysis.

## Model Development

### Machine Learning Models
We implemented the following machine learning models to predict the sales price of properties:
- **Linear Regression**: A baseline model to understand the relationship between the features and the target variable.
- **Random Forest Regressor**: A more complex model to capture non-linear relationships in the data.
- **XGBoost Regressor**: A gradient boosting model known for its high performance in regression tasks.

### Model Evaluation
We evaluated the models using performance metrics such as **Mean Absolute Error (MAE)**, **Mean Squared Error (MSE)**, and **R-squared (R2)** to select the best model for prediction.

## Conclusion
The project successfully built a predictive model for estimating the sales prices of residential properties in Chennai. Key insights from the data were uncovered through exploratory data analysis, which helped improve the model's understanding of property prices. The final model is capable of predicting sales prices with a high level of accuracy and can be used for property valuation purposes.

## Future Work
- Incorporate additional features like property amenities and more granular data on property conditions.
- Further tuning of the models and exploration of other regression techniques could improve predictive performance.

