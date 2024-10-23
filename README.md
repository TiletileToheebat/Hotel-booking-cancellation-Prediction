# **Hotel Booking Cancellation Prediction**
This project focuses on predicting whether a hotel guest will cancel their reservation based on a variety of features such as lead time, stay duration, customer type, and more. By analyzing historical data and applying machine learning models, this project aims to provide insights into factors that contribute to cancellations, and predict future cancellations with a good level of accuracy.

## **Project Overview**
Hotel booking cancellation can significantly impact revenue and operations. Using a dataset with multiple worksheets containing booking details, meal costs, and market segment discounts, this project builds predictive models to classify reservations as either canceled or not canceled.

### **Steps in the Project:**
1. **Data Loading and Preprocessing**: 
   - Loaded datasets from five worksheets containing hotel booking information for the years 2018, 2019, and 2020.
   - Merged and concatenated the worksheets.
   - Handled missing values by replacing or dropping them appropriately.
   - Removed outliers using the IQR method.

2. **Exploratory Data Analysis**:
   - Checked data structure and summary statistics.
   - Visualized distributions using histograms, box plots, and bar charts.
   - Analyzed categorical and numerical variables and their relationship to the cancellation status.

3. **Feature Engineering**:
   - Encoded categorical data and performed feature selection.
   - Selected important features excluding irrelevant columns like reservation status and arrival date year.

4. **Model Development**:
   - Split data into training and testing sets.
   - Applied three classification models:
     - Logistic Regression: 78.44% accuracy
     - Decision Tree Classifier: 82.25% accuracy
     - Random Forest Classifier: 86.53% accuracy

5. **Feature Importance**:
   - Identified top 10 features contributing to booking cancellations, including:
     - Country
     - Lead time
     - adr
     -  arrival_date_day_of    0.070417
     -  arrival_date_week    0.062921
     - arrival_date_month    0.058540
     - total_of_special    0.057633
     - agent    0.048794
     - stays_in_week    0.047177
     - market_segment

## **Key Results**:
- The **Random Forest Classifier** outperformed the other models with an accuracy of **86.53%**.
- The most important features for predicting cancellations include lead time, agent, and adr.

## **Technologies Used**:
- Python
- Pandas
- Scikit-learn
- Matplotlib
- Seaborn

## **How to Use**:
1. Clone this repository.
2. Install the required dependencies from `requirements.txt`.
3. Run the Jupyter Notebook to see the data analysis and model development in action.
