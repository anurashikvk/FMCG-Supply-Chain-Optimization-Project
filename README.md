# Fast Moving Consumer Goods (FMCG) Supply Chain Management Project 🌐📈

## Company Overview 🏭
The project focuses on a leading FMCG company that entered the instant noodles market two years ago. Identifying a significant issue of mismatch between demand and supply, leading to inventory costs and overall losses, the management aims to optimize the supply quantity in each warehouse nationwide.

## Data Overview 📊🔍
The dataset includes information about warehouses, managers, regional zones, and various factors affecting the supply chain. The primary challenge is addressing the mismatch in demand and supply to reduce inventory costs and losses.

## Problem Solving Approach 🛠️💡

### 1. Exploratory Data Analysis (EDA)
- **Description:** Dive into the dataset to understand its structure, identify patterns, and uncover insights into the business. EDA serves as the foundation for subsequent data cleaning and feature engineering steps.

### 2. Data Cleaning 🧹🔧
- **Description:** Ensure the dataset's integrity and prepare it for analysis by addressing missing values and removing unnecessary columns.
   - *Delete unnecessary columns:* Remove features that do not contribute significantly to the analysis.
   - *Checking missing values:* Identify and handle missing data.
   - *Filling missing values in the 'workers_num' column:* Address missing values using the mean value of the column.
   - *Discard the 'wh_est_year' column:* Remove a column with a high percentage of null values.
   - *Filling missing values in the 'approved_wh_govt_certificate' column:* Fill missing values with the most recent non-null value.

### 3. Data Visualization 📊
- **Description:** Create visual representations of the data to gain insights and understand key relationships.
   - *Warehouse count by WH_capacity_size:* Visualize the distribution of warehouses based on capacity size.
   - *WH_capacity_size by Location_type:* Explore how capacity size varies across different location types.
   - *WH_capacity_size by zone:* Analyze the relationship between capacity size and zones.
   - *Warehouse count by WH_regional_zone:* Understand the distribution of warehouses across regional zones.

### 4. Feature Engineering
- **Description:** Enhance the dataset by creating new features or modifying existing ones to improve model performance.
   - *Product weights by zone:* Derive new features related to product weights based on regional zones.
   - *Heatmap for correlation matrix:* Visualize relationships between different features using a heatmap.
   - *Correlation with the target variable:* Examine the correlation between various features and the target variable.

### 5. Data Preprocessing 🌐🔍
- **Description:** Prepare the data for modeling by encoding categorical variables and scaling numerical features.
   - *Encode 'Location_type' column:* Transform categorical location types into numerical representations.
   - *Encode 'WH_capacity_size' column:* Convert warehouse capacity sizes into numerical labels.
   - *Encode 'approved_wh_govt_certificate' column:* Encode approval status for government certificates.
   - *Encode 'zone' column:* Numerically represent different zones.
   - *Encode 'WH_regional_zone' column:* Encode regional zones.
   - *Encode 'wh_owner_type' column:* Convert warehouse owner types into numerical labels.

### 6. Model Building 🛠️📈
Implementing various machine learning models to predict the optimum product weight:

- **Linear Regression:** A simple linear model for predicting weights based on historical data.
- **Decision Tree:** A tree-based model for capturing complex relationships in the data.
- **Random Forest:** An ensemble model combining multiple decision trees for improved accuracy.
- **SVR (Support Vector Regression):** A model for capturing non-linear relationships in the data.
- **XGBoost:** An efficient gradient boosting model for regression tasks.
- **Neural Network:** A deep learning model for complex pattern recognition and prediction.

![Screenshot 2024-01-29 232604](https://github.com/anurashikvk/FMCG-Supply-Chain-Optimization-Project/assets/134492695/4819daa6-61b7-4d46-997c-91818df14e38)


![modal comparison](https://github.com/anurashikvk/FMCG-Supply-Chain-Optimization-Project/assets/134492695/410fc37b-7fcb-4ec6-ad04-d32cce368e61)



### 7. Next Steps 🚀
Description: Continuous improvement and refinement of the model can be achieved through:

Gathering more data: Expanding the dataset with additional relevant information.

Fine-tuning hyperparameters: Adjusting model parameters for optimal performance.

Cross-validation: Ensuring the model's robustness by evaluating it on different subsets of the data.

Model interpretation: Understanding the model's decisions and adjusting accordingly.

### 8. Improvements 🌱
Description: Considerations for enhancing the project further:

Real-time data integration: Implementing a mechanism to incorporate live data for up-to-date predictions.

Deployment: Transitioning the model from development to production for practical usage.

User interface: Developing a user-friendly interface for easy interaction with the supply chain predictions.

Feedback loop: Establishing a feedback mechanism to continuously improve the model based on real-world outcomes.

---
