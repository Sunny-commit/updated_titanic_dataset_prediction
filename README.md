🚢 Titanic Survival Prediction – Enhanced ML Pipeline
Welcome aboard the Titanic machine learning project! 🎯
In this upgraded version, we take a classic dataset and go beyond the basics — with thorough preprocessing, EDA, feature engineering, and comparison across multiple powerful classifiers.

📁 Dataset Overview
This project uses the famous Titanic dataset (Titanic.csv) containing details of passengers, such as:

Demographics: Age, Sex, Embarked

Travel Info: Pclass, Fare, Ticket, Cabin

Family: SibSp, Parch

Target: Survived (0 = No, 1 = Yes)

🔍 1. Data Preprocessing
We started by filling missing values smartly:

Age: filled with mean

Cabin, Embarked: filled with mode

We also:

Dropped irrelevant or high-cardinality columns like Name, Cabin, and Ticket

Applied log transformation to fix skewness in Fare

Used Label Encoding on categorical features (Sex, Embarked)

📊 2. Exploratory Data Analysis (EDA)
We visualized:

Distribution of age, fare, and survival

Class distributions using countplot

Correlation matrix using a heatmap for insights on key features

This helps us understand which features most influence survival.

⚙️ 3. Model Building
Multiple models were trained and compared for accuracy:

Model	Accuracy (approx.)
Logistic Regression	✅ Baseline model
Decision Tree	🌲 Interpretable
Random Forest	🌳 Ensemble power
Extra Trees Classifier	🌟 Fast & accurate
XGBoost	🔥 High performance
LightGBM	⚡ Fast & efficient
CatBoost	🐱 Handles categories well
Each model was tested with train_test_split and evaluated by .score() and cross_val_score().

✅ 4. Final Deployment Model
After comparing models, LightGBM (LGBMClassifier) was selected as the final model. It was retrained on the full dataset for final predictions.

🛠️ Tools & Libraries Used
Python 🐍

pandas, numpy – for data manipulation

seaborn, matplotlib – for visualization

scikit-learn – ML models and preprocessing

xgboost, lightgbm, catboost – advanced boosting libraries

▶️ How to Run
Make sure the file Titanic.csv is available in your working directory (or Colab environment).

Run titanic_dataset (1).py.

Check out the visualizations and compare model accuracies.

You’ll see predictions and evaluation results right in the output.
