Car Price Prediction (Regression)

This project was developed as part of my remote internship at CodeAlpha. It aims to predict the selling price of used cars using machine learning regression techniques, particularly XGBoost Regressor. This model helps identify how factors like car age, fuel type, ownership, and driven kilometers affect the resale value of a car.

1. 📁 Project Structure
notebooks/
├── Car_Price_Prediction_Regression.ipynb   # Main notebook
├── cardata.csv                             # Dataset
├── result.png                              # Model output visualization
├── Way.png                                 # Data pipeline or project flow image

2. 🎯 Objectives

Understand which car features influence the selling price.

Train a regression model to predict selling prices.

Visualize and evaluate the model performance.

3. 🧠 Technologies Used

Python

Pandas and NumPy – data manipulation

Matplotlib, Seaborn, Plotly – data visualization

Scikit-learn – preprocessing, model evaluation

XGBoost – regression model

GitHub – version control and sharing

4. 🗃️ Dataset

Filename: cardata.csv

Columns included:

Car_Name

Year

Selling_Price

Present_Price

Driven_kms

Fuel_Type

Selling_type

Transmission

Owner

We added an engineered column Car_Age = 2025 - Year for better feature understanding.

5. 🔍 Exploratory Data Analysis (EDA)

Checked for missing values and duplicates.

Added feature: Car_Age

Visualized relationships:

Present_Price vs. Selling_Price

Fuel type distribution

Depreciation percentage per car

Summarized depreciation insights and car performance statistics.

6. 🔧 Preprocessing

Converted categorical variables using One-Hot Encoding

Split data into train/test sets using train_test_split

Handled feature mismatch using reindex for test set alignment

7. 🧪 Model Training

Model: XGBRegressor

Metric used:

RMSE (Root Mean Squared Error)

R² Score

Result:

RMSE ≈ low value (indicating good fit)

R² ≈ high value (close to 1)

8. 📊 Visualization

Scatter plot of Actual vs. Predicted Price

Bar charts of fuel types, transmission, and ownership counts

Interactive depreciation graphs using Plotly

9. 🔮 Price Prediction

A separate input section allows predicting a car’s selling price based on:

Year

Present Price

Kms Driven

Owner type

Fuel Type

Transmission

Car Name

💡 After fixing feature mismatch issues, the prediction output is realistic and dynamic for each input combination.

10. ✅ Key Takeaways

Car price prediction can be enhanced by including Car_Age, ownership type, and present price.

XGBoost provides a good fit for regression in automotive datasets.

Proper one-hot encoding and matching input features with model training columns are critical.

11. 📌 Next Steps

Add UI using Streamlit or Flask

Use real-time user inputs for predictions

Tune hyperparameters with GridSearchCV

Save model using joblib for deployment

12. 📷 Snapshots

result.png: Actual vs. Predicted Price Plot

Way.png: Project pipeline overview

13. 👤 Author

Name: Zaighum Jawad Aslam

Internship: CodeAlpha – Remote Data Science Internship

GitHub: github.com/ZaighiChohan
