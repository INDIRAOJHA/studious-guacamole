**Telecom Churn Data Analysis**

**Overview**

This project involves the analysis of telecom customer data to understand their behavior and to potentially build predictive models. The dataset contains a wide variety of features related to customer mobile usage, service types, and recharge behavior over different months.

**Dataset**

- **File Name**: telecom churn data.csv
- **Dataset Description**: The dataset contains 226 features related to customers’ mobile usage patterns, service types, and engagement levels across different months. The target variable (churn status) is not explicitly mentioned, but useful insights can still be drawn based on customer behavior over time.
  - **Key Features**:
    - mobile_number: Unique identifier for each customer
    - circle_id: Geographical circle ID where the customer is located
    - loc_og_t2o_mou, std_og_t2o_mou: Outgoing minutes of usage for local and standard calls
    - arpu_6, arpu_7, arpu_8, arpu_9: Average revenue per user over the months (June to September)
    - fb_user_6, fb_user_7, fb_user_8, fb_user_9: Whether the user accessed Facebook services during the respective months
    - aon: Age on network (in days)
    - aug_vbc_3g, jul_vbc_3g, jun_vbc_3g, sep_vbc_3g: Volume-based charges for 3G services over different months

**Problem Statement**

The goal is to analyze customer behavior and identify trends or patterns that could indicate customer disengagement or churn. The dataset provides valuable information for customer segmentation and revenue analysis.

**Project Workflow**

1. **Exploratory Data Analysis (EDA)**:
    - **Univariate Analysis**: Histograms and box plots for numerical columns like arpu, aon, and minutes of usage.
    - **Bivariate Analysis**: Correlation heatmap, scatter plots for understanding relationships between different usage metrics and revenue.
    - **Multivariate Analysis**: Investigating trends across multiple variables, such as how usage patterns across months change based on circle_id.
2. **Data Preprocessing**:
    - **Handling Missing Values**: Dealing with missing values in columns such as fb_user_6, fb_user_7, and others.
    - **Outlier Treatment**: Detecting and treating outliers in columns such as arpu and usage metrics.
    - **Encoding Categorical Features**: Encoding variables like circle_id that represent categorical data.
    - **Scaling Numerical Features**: Features like arpu, aon, and usage data are scaled using techniques like **Min-Max Scaling** or **Standardization**.
3. **Insights Generation**:
    - **Customer Segmentation**: Segmenting customers based on their usage patterns and revenue contributions.
    - **Revenue Analysis**: Identifying high and low revenue-generating customers based on their arpu values.
4. **Installation and Requirements**

To run this analysis, ensure you have the following dependencies installed:

**Key Libraries:**

- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

**Results and Insights**

- Customer usage patterns and revenue contributions were analyzed, leading to potential customer segmentation.
- Average revenue per user (ARPU) showed strong variation across months, which can help in identifying customers who may need retention efforts.
