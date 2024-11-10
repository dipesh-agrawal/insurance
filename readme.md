# Insurance Premium Prediction  
  
This project aims to analyze and predict insurance premium prices based on various factors such as age, BMI, diabetes, blood pressure problems, and other health conditions. The analysis and model training are conducted using a dataset uploaded to Google Colab.  
  
## Table of Contents  
- [Installation](#installation)  
- [Data Analysis](#data-analysis)  
- [Statistical Tests](#statistical-tests)  
- [Model Training](#model-training)  
- [Model Evaluation](#model-evaluation)  
- [Streamlit App](#streamlit-app)  
- [Link to Streamlit App](#link-to-streamlit-app)  
- [Conclusion](#conclusion)  

  
## Installation  
  
To run the notebook and the Streamlit app, you need to install the following dependencies:  
  
- pandas  
- matplotlib  
- seaborn  
- scipy  
- scikit-learn  
- xgboost  
- streamlit  
- pyngrok  
  
## Data Analysis  
  
1. **Upload the Dataset**: The dataset is uploaded and read into a pandas DataFrame.  
2. **Check for Null Values**: Sum of null values in each column is checked to handle missing data.  
3. **Correlation Heatmap**: A heatmap is created to visualize the correlation between different features.  
4. **Descriptive Statistics**: Descriptive statistics of the dataset are generated for an overview.  
  
## Statistical Tests  
  
1. **T-test for Diabetes**: A two-sample t-test is performed to compare the mean premium prices between individuals with and without diabetes.  
2. **T-test for Blood Pressure Problems**: A two-sample t-test is performed to compare the mean premium prices between individuals with and without blood pressure problems.  
3. **ANOVA for Age Groups**: ANOVA is performed to compare the mean premium prices among different age groups.  
4. **Chi-square Test for Diabetes and Cancer History**: A chi-square test is performed to check the association between diabetes and history of cancer in the family.  
5. **Mann-Whitney U Test for Chronic Diseases**: A Mann-Whitney U test is performed to compare the premium prices between individuals with and without chronic diseases.  
  
## Model Training  
  
### Random Forest Model with Grid Search  
  
1. **Grid Search**: Grid search with cross-validation is performed to find the best hyperparameters for the Random Forest model.  
2. **Train the Best Model**: The best model from grid search is trained on the training data.  
  
## Streamlit App  
  
A Streamlit app is created to provide a user interface for predicting insurance premium prices based on user input parameters. The app includes:  
  
1. **Sidebar for User Input**: Users can input their details such as age, BMI, diabetes, blood pressure problems, etc.  
2. **Load Pre-trained Model**: The pre-trained model is loaded to make predictions based on user input.  
3. **Display User Input**: The app displays the input parameters entered by the user.  
4. **Predict Premium Price**: When the user clicks the "Predict" button, the app predicts the insurance premium price based on the input parameters and displays the result.  
  
## Streamlit App Deployment  
  
To deploy the Streamlit app, the following steps are taken:  
  
1. **Set up ngrok**: ngrok is used to create a public URL for the Streamlit app, allowing it to be accessed from the internet.  
2. **Run Streamlit App**: The Streamlit app is started, and ngrok provides a public URL where the app can be accessed.  
  
## Link to Streamlit App  
  
[Link](https://6d21-35-236-155-128.ngrok-free.app/) 
  
## Conclusion  
  
This project demonstrates the process of analyzing, training, and evaluating machine learning models for predicting insurance premium prices. Various statistical tests are performed to understand the relationships between different features and the premium prices. The trained models are then deployed using a Streamlit app, allowing users to input their details and get a predicted premium price.  
