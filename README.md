E-commerce Marketing Budget Optimization & Sales Prediction
This project focuses on optimizing the marketing budget for an e-commerce firm based in Ontario, Canada, which specializes in electronic products. The goal is to build machine learning (ML) and deep learning (DL) models to predict weekly sales for three product subcategories — camera accessory, home audio, and gaming accessory. Additionally, the project aims to analyze how external factors like weather conditions affect sales, enabling the firm to strategically allocate marketing spend for maximum impact.

Data preparation: Integrating sales, product, and weather data for the Ontario region from 2015 and 2016.
Feature engineering: Creating features such as pay dates, holidays, and climate indicators (e.g., temperature, precipitation).
Exploratory Data Analysis (EDA): Performing univariate and bivariate analyses, correlation studies, and visualizations.
Modeling: Building machine learning and deep learning models to predict weekly sales for each subcategory and understanding the impact of weather on sales.
Optimization: Using the insights from the models to optimize the marketing budget by reallocating resources to improve revenue response.

Key Files:
data_preparation.ipynb: Notebook for data loading, cleaning, and merging.
exploratory_analysis.ipynb: Notebook for exploratory data analysis (EDA).
modeling_ml.ipynb: Notebook for machine learning models.
modeling_dl.ipynb: Notebook for deep learning models.

Weather Reports (2015, 2016): Climate data (temperature, precipitation) for Ontario.
Product Details: Information about products, including categories, subcategories, and verticals.
Purchase Frequency: Frequency and percentage of product purchases.
Sales Data: Sales transactions, including order details, units sold, and gross merchandise value (GMV).

Sales data: gmv, units, order_date, order_payment_type
Product details: product_analytic_sub_category, product_mrp
Weather data: Mean Temp (°C), Total Rain (mm), Total Snow (cm)
Other: pay_date, holiday_flag, week

Feature Engineering
Key engineered features include:
avg_temp: Average temperature per day.
pay_date: Indicator for paydays (1st and 15th of the month).
holiday_flag: Binary flag for holidays.
week: Aggregated weekly sales data.

Exploratory Data Analysis (EDA)
Key analyses include:
Univariate analysis: Distribution of key variables like gmv, units, and avg_temp.
Bivariate analysis: Relationship between temperature and sales across product subcategories.
Correlation analysis: Insights on how weather data correlates with sales.

Modeling
We developed the following models to predict sales and assess the impact of weather:
Machine Learning Models:
Linear Regression
Decision Tree Regressor
Random Forest Regressor
Deep Learning Models:
Multilayer Perceptron (MLP) using Keras/TensorFlow
Metrics:
R² (Coefficient of Determination): Explains the variance captured by the model.


Requirements
The project dependencies are listed in requirements.txt. Key libraries include:
pandas
numpy
matplotlib
seaborn
scikit-learn
tensorflow


Results
The analysis showed that:
Temperature has a significant effect on sales, especially for camera accessories and home audio categories.
Rainy and cold days tend to see higher sales in certain subcategories, suggesting a potential trend in consumer behavior during such weather conditions.
The model achieved an R² score of 0.98 for predicting weekly sales, indicating a good fit between temperature and sales data.

Future Improvements
Incorporate additional marketing data: Include marketing spend, promotions, and advertisement effectiveness to refine the model.
Seasonality and trend analysis: Analyze long-term trends and cyclical patterns in the data.
Refine deep learning models: Tune hyperparameters and explore more complex architectures.
