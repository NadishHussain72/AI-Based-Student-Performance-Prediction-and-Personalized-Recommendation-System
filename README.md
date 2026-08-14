# 🎓 AI-Based Student Performance Prediction and Personalized Recommendation System

## 📌 Project Overview

The **AI-Based Student Performance Prediction and Personalized Recommendation System** is an intelligent Artificial Intelligence project that predicts student academic performance and provides personalized recommendations for improvement.

The system analyzes academic and behavioral factors such as study hours, attendance, previous exam scores, assignment scores, quiz scores, sleep hours, participation, and completed assignments.

Instead of only predicting a student's performance, the system also identifies areas that may need improvement and provides personalized recommendations.

---

## 🎯 Project Objectives

The main objectives of this project are:

* Predict student academic performance using AI/ML.
* Preprocess and analyze student data.
* Compare multiple machine learning models.
* Implement an Artificial Neural Network.
* Classify students according to their performance level.
* Provide personalized recommendations.
* Visualize model and dataset results.
* Build an interactive user interface.

---

## 🧠 AI Models Used

The project uses three different AI/ML models:

### 1. Random Forest

A Random Forest classifier is used to predict student performance based on multiple academic and behavioral features.

### 2. XGBoost

XGBoost is used as a powerful gradient boosting model and is compared with Random Forest and the Neural Network.

### 3. Artificial Neural Network

The project also implements a Neural Network with the following architecture:

```text
Input Layer
     ↓
64 Neurons
     ↓
32 Neurons
     ↓
16 Neurons
     ↓
Output Layer
```

The network uses the **ReLU activation function** and the **Adam optimizer**.

---

## 📊 Input Features

The system uses the following features:

| Feature               | Description                     |
| --------------------- | ------------------------------- |
| Study Hours           | Average study hours per day     |
| Attendance            | Student attendance percentage   |
| Previous Score        | Previous examination score      |
| Assignment Score      | Assignment performance          |
| Quiz Score            | Quiz performance                |
| Sleep Hours           | Average daily sleep             |
| Participation         | Class participation level       |
| Completed Assignments | Number of completed assignments |

---

## 🎯 Prediction Categories

The AI system classifies students into four performance categories:

```text
🔴 At Risk
🟡 Average
🔵 Good
🟢 Excellent
```

The system also provides:

* Estimated performance score
* AI confidence
* Risk level
* Individual model predictions
* Personalized recommendations

---

## 🔄 System Workflow

```text
Student Data
     ↓
Data Preprocessing
     ↓
Feature Selection
     ↓
Train/Test Split
     ↓
Feature Scaling
     ↓
 ┌─────────────────┐
 │ Random Forest   │
 └────────┬────────┘
          │
 ┌────────▼────────┐
 │    XGBoost      │
 └────────┬────────┘
          │
 ┌────────▼────────┐
 │ Neural Network  │
 └────────┬────────┘
          ↓
 Model Comparison
          ↓
 Final Prediction
          ↓
 Risk Classification
          ↓
 AI Recommendation
          ↓
 Interactive Interface
```

---

## 🧹 Data Preprocessing

The project performs several preprocessing steps:

* Removes duplicate records.
* Checks for missing values.
* Handles missing numerical values using the median.
* Separates input features and target variable.
* Splits the dataset into training and testing sets.
* Applies `StandardScaler` for neural network training.

---

## 📈 Data Visualization

The project includes multiple visualizations:

* Correlation heatmap
* Student performance distribution
* Model accuracy comparison
* Confusion matrix
* Feature importance
* Neural Network training loss
* Model evaluation metrics

These visualizations help understand the dataset and evaluate the AI models.

---

## 💡 Intelligent Recommendation System

The recommendation engine analyzes individual student information and generates personalized suggestions.

For example:

### Low Attendance

```text
Your attendance is low.
Try to attend classes regularly to improve your understanding.
```

### Low Study Hours

```text
Increase your daily study time to approximately 2–4 hours.
```

### Low Quiz Score

```text
Practice more quizzes and review the topics where you lose marks.
```

### Low Assignment Performance

```text
Complete assignments regularly and submit them on time.
```

The recommendations are generated according to the student's actual input values.

---

## 🖥️ User Interface

The project includes an interactive **Gradio interface**.

Users can enter:

* Study hours
* Attendance
* Previous score
* Assignment score
* Quiz score
* Sleep hours
* Participation
* Completed assignments

After clicking **Predict Performance**, the system displays:

```text
Final Performance
Estimated Score
AI Confidence
Risk Level

Random Forest Prediction
XGBoost Prediction
Neural Network Prediction

Personalized Recommendations
```

The interface uses a **burgundy and white visual theme**.

---

## 🛠️ Technologies Used

### Programming Language

* Python

### Data Processing

* Pandas
* NumPy

### Machine Learning

* Scikit-learn
* Random Forest
* XGBoost

### Deep Learning

* Artificial Neural Network
* MLPClassifier

### Visualization

* Matplotlib
* Seaborn

### User Interface

* Gradio

### Development Environment

* Google Colab
* Jupyter Notebook

---

## 📁 Project Structure

```text
AI_Student_Performance_System/
│
├── student_performance.csv
│
├── AI_Student_Performance.ipynb
│
├── README.md
│
└── Gradio Interface
```

---

## 🚀 How to Run the Project

### Step 1 — Open Google Colab

Open a new Google Colab notebook.

### Step 2 — Install Libraries

Run:

```bash
!pip install -q xgboost seaborn scikit-learn pandas numpy matplotlib gradio
```

### Step 3 — Run the Notebook

Run the cells in order:

```text
1. Project Introduction
2. Library Installation
3. Import Libraries
4. Dataset Generation
5. Dataset Saving
6. Dataset Display
7. Dataset Information
8. Missing Value Checking
9. Data Preprocessing
10. Exploratory Data Analysis
11. Performance Distribution
12. Feature Selection
13. Train/Test Split
14. Feature Scaling
15. Random Forest
16. Random Forest Evaluation
17. XGBoost
18. Neural Network
19. Neural Network Visualization
20. Model Comparison
21. Accuracy Visualization
22. Confusion Matrix
23. Feature Importance
24. Feature Importance Visualization
25. Evaluation Metrics
26. Recommendation Engine
27. Prediction Function
28. Test Prediction
29. Interactive Prediction
30. Recommendations
31. Final Dashboard
32. Gradio Interface
```

---

## 📊 Model Evaluation

The project compares the performance of:

```text
Random Forest
XGBoost
Neural Network
```

The evaluation includes:

* Accuracy
* Precision
* Recall
* F1 Score
* Confusion Matrix

**Note:** Model performance values depend on the dataset and training/testing split. The accuracy values should be reported from the actual execution of the notebook rather than using illustrative values.

---

## 🎓 Academic Requirements Covered

This project covers the major requirements of the AI Week 6 Final Project:

| Requirement           | Implementation                      |
| --------------------- | ----------------------------------- |
| AI/ML Model           | Random Forest & XGBoost             |
| Data Preprocessing    | Missing values, duplicates, scaling |
| Prediction System     | Student performance prediction      |
| Recommendation System | Personalized recommendations        |
| Neural Network        | Multi-layer ANN                     |
| Visualization         | Multiple graphs and charts          |
| User Interaction      | Gradio interface                    |
| AI Decision Making    | Risk classification                 |
| Model Evaluation      | Accuracy, Precision, Recall, F1     |
| Complete AI Project   | End-to-end AI system                |

---

## 🔮 Future Improvements

The project can be further improved by:

* Using a real-world student dataset.
* Adding previous GPA as an input feature.
* Adding internet/resource availability.
* Using TensorFlow/Keras for a deeper neural network.
* Adding explainable AI using SHAP.
* Saving trained models using Joblib.
* Deploying the application online.
* Adding a student login system.
* Adding historical performance tracking.
* Providing subject-specific recommendations.

---

## 👨‍💻 Project Information

**Project Title:**
AI-Based Student Performance Prediction and Personalized Recommendation System

**Project Type:**
Artificial Intelligence / Machine Learning


**Environment:**
Google Colab

**Interface:**
Gradio

---

## 📜 Conclusion

The **AI-Based Student Performance Prediction and Personalized Recommendation System** demonstrates a complete AI workflow, starting from data preprocessing and feature engineering and continuing through machine learning, neural networks, model evaluation, prediction, visualization, and intelligent recommendations.

The project demonstrates how AI can be applied to educational data to predict student performance and provide useful, personalized academic guidance.
