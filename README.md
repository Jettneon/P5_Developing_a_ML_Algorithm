# Heart Disease Prediction - Machine Learning Project

This project aims to predict whether a patient has a heart disease or not based on various features like age, gender, chest pain type, blood pressure, and others. The data is sourced from a database containing multiple tables that are joined to form the final dataset. The machine learning model used for prediction is Logistic Regression.

## Project Structure

├── heart_data.csv # The dataset used for training the model ├── notebook.ipynb # Jupyter notebook with all analysis and model training ├── requirements.txt # File containing all dependencies └── README.md # Project documentation


## Task

1. **Import the Data**: Download the data from the database. The schema is called `heart`. Use DBeaver to inspect the tables and join them appropriately.
2. **Exploratory Data Analysis (EDA)**: Conduct a brief exploratory analysis to get familiar with the data.
3. **Preprocess the Data**: Clean and preprocess the data as needed (handling missing values, scaling, encoding, etc.).
4. **Train a Logistic Regression Model**: Use the preprocessed data to train a Logistic Regression model to predict heart disease.

## Features

- **age**: Age of the patient
- **sex**: Gender of the patient
- **chest_pain_type**: Type of chest pain (1 = typical angina, 2 = atypical angina, 3 = non-anginal pain, 4 = asymptomatic)
- **resting_blood_pressure**: Blood pressure at rest
- **fasting_blood_sugar**: Whether the fasting blood sugar is > 120 mg/dl (1 = true, 0 = false)
- **thal**: Thalassemia (0 = normal, 1 = fixed defect, 2 = reversible defect)
- **serum_cholestoral**: Serum cholesterol in mg/dl
- **resting_electrocardiographic_results**: Electrocardiogram results (0 = normal, 1 = abnormal ST-T wave, 2 = left ventricular hypertrophy)
- **maximum_heartrate_achieved**: Maximum heart rate achieved during exercise
- **exercise_induced_angina**: Whether the patient has angina induced by exercise (1 = yes, 0 = no)
- **oldpeak**: ST depression induced by exercise relative to rest
- **slope_of_the_peak_exercise_st_segment**: Slope of the peak exercise ST segment (1 = upsloping, 2 = flat, 3 = downsloping)
- **number_of_major_vessels_colored_by_flourosopy**: Number of major vessels colored by fluoroscopy
- **real_data**: Tag indicating whether the data is real or synthetic
- **heart_attack**: 0 = little risk, 1 = high risk

## Steps Involved

### 1. Import Data
Use SQLAlchemy to connect to the PostgreSQL database and import the dataset into the notebook.

### 2. Preprocessing
Handle missing values, perform feature scaling, encode categorical variables, and split the dataset into training and testing sets.

### 3. Train Model
Train a Logistic Regression model and evaluate its performance using relevant metrics like accuracy, precision, recall, and F1 score.

### 4. Hyperparameter Tuning
Use RandomizedSearchCV and GridSearchCV for hyperparameter tuning of the Logistic Regression model.

## Evaluation Metrics
- **Accuracy**: The proportion of correct predictions.
- **Precision**: The proportion of positive predictions that were actually positive.
- **Recall**: The proportion of actual positive cases that were correctly identified.
- **F1 Score**: The harmonic mean of precision and recall.

## How to Use
To replicate the analysis or use the code for your own projects, follow these steps:
1. Clone the repository to your local machine.
   ```bash
   git clone https://github.com/your-username/Developing_a_ML_Algorithm.git


2. Install required libraries using pip.
   ```bash 
    pip install -r requirements.txt

3. Open the Jupyter notebook to begin the analysis.
   ```bash 
    jupyter notebook Developing_ML_Algorithm.ipynb
    ```

## Technologies Used
- **Python**: The primary programming language for data analysis and machine learning.
- **Pandas**: For data manipulation and analysis.
- **NumPy**: For numerical operations and data handling.
- **Matplotlib/Seaborn**: Data visualization libraries for creating insightful plots.
- **SQLAlchemy**: For connecting to the PostgreSQL database and importing data.
- **Scikit-learn**: For machine learning models, evaluation metrics, and preprocessing steps like scaling.


License
This project is licensed under the MIT License - see the LICENSE file for details.



### Key Markdown Elements:
- `#` for top-level headers.
- `##` for secondary-level headers.
- `-` for unordered lists.
- Code blocks (such as for installation commands) are enclosed with triple backticks: ```bash ... ```.
- Links are formatted with `[link text](URL)`.
- Bold text is wrapped in `**`, like `**text**`.

You can now copy and paste this into your `README.md` file, and it should render properly on GitHub with the correct formatting. Let me know if you need any further assistance!
