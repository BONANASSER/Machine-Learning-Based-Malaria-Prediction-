# Machine-Learning-Based-Malaria-Prediction
🎯 Project Objectives

Develop predictive models for malaria diagnosis

Compare multiple machine learning classification algorithms

Improve prediction performance through data preprocessing techniques

Identify the most influential clinical features affecting malaria infection

📊 Dataset Description

The dataset contains patient clinical and demographic information, including:

Age

Gender

Pregnancy status

Body temperature

Travel history

Previous malaria infection history

⚙️ Data Preprocessing

The following preprocessing techniques were applied:

Data cleaning

Handling missing values

Categorical feature encoding

Feature normalization

Class imbalance handling using SMOTE (Synthetic Minority Oversampling Technique)

Train–test data splitting

🤖 Machine Learning Models Used

The following classification algorithms were implemented and evaluated:

Logistic Regression

Decision Tree

K-Nearest Neighbor (KNN)

Artificial Neural Network (ANN)

Random Forest

Support Vector Machine (SVM)

📈 Model Performance
Model	Accuracy
Decision Tree	100%
Random Forest	100%
Artificial Neural Network	99.09%
Support Vector Machine	94.54%
KNN	88.18%
Logistic Regression	85.45%
⭐ Feature Importance

Feature importance analysis revealed that the most influential predictors were:

Body temperature

Travel history

Previous malaria infection history

These features significantly contributed to the model’s prediction capability.

💡 Key Contributions

Demonstrates the effectiveness of machine learning in malaria prediction

Provides a comparative evaluation of multiple classification algorithms

Supports early diagnosis using readily available clinical data

Offers a potential decision-support tool for healthcare workers

🛠️ Technologies Used

Python

Pandas

NumPy

Scikit-learn

Matplotlib / Seaborn

Imbalanced-learn (SMOTE)

🚀 How to Run the Project
# Clone repository
git clone https://github.com/yourusername/malaria-prediction.git

# Navigate into project folder
cd malaria-prediction

# Install dependencies
pip install -r requirements.txt

# Run the model
python malaria_prediction.py
📍 Future Improvements

Use larger real-world datasets

Deploy as a web or mobile application

Integrate real-time clinical data

Apply deep learning and ensemble optimization techniques

📚 References

World Health Organization (WHO) Malaria Reports

Machine Learning Applications in Healthcare Research

👤 Author

Bona Nasser
MSc in Data Science
Haramaya University, Ethiopia
