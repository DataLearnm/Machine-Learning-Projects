# 🌸 Iris Flower Classification using Logistic Regression

## 📌 Project Overview

This project demonstrates a simple and effective implementation of **Logistic Regression** to classify iris flowers into three species:

* Setosa
* Versicolor
* Virginica

The model is trained on the famous Iris dataset and predicts the species based on four features:

* Sepal Length
* Sepal Width
* Petal Length
* Petal Width

---

## 🎯 Objectives

* Understand classification using Logistic Regression
* Perform data preprocessing and visualization
* Train and evaluate a machine learning model
* Predict flower species based on input features

---

## 📂 Dataset

The dataset used is the **Iris dataset**, which contains 150 samples with 4 features each and 3 target classes.

---

## 🛠️ Technologies Used

* Python
* NumPy
* Pandas
* Matplotlib / Seaborn
* Scikit-learn

---

## ⚙️ Installation

Clone the repository and install required dependencies:

```bash
git clone https://github.com/your-username/iris-logistic-regression.git
cd iris-logistic-regression
pip install -r requirements.txt
```

---

## 🚀 Usage

Run the Python script to train and test the model:

```bash
python app.py
```

---

## 🧠 Model Implementation

Steps involved:

1. Load dataset
2. Explore and visualize data
3. Split data into training and testing sets
4. Train Logistic Regression model
5. Evaluate model performance using accuracy and confusion matrix

---

## 📊 Results

* Achieved high accuracy on test data
* Model performs well in distinguishing between all three classes

---

## 📈 Sample Code

```python
from sklearn.datasets import load_iris
from sklearn.model_selection import train_test_split
from sklearn.linear_model import LogisticRegression
from sklearn.metrics import accuracy_score

# Load dataset
iris = load_iris()
X = iris.data
y = iris.target

# Split data
X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2, random_state=42)

# Train model
model = LogisticRegression(max_iter=200)
model.fit(X_train, y_train)

# Predictions
y_pred = model.predict(X_test)

# Accuracy
print("Accuracy:", accuracy_score(y_test, y_pred))
```

---

## 🔍 Evaluation Metrics

* Accuracy Score
* Confusion Matrix
* Classification Report

---

## 📌 Future Improvements

* Hyperparameter tuning
* Cross-validation
* Deploy model using Flask or Streamlit
* Add user interface for predictions

---

## 🤝 Contributing

Contributions are welcome! Feel free to fork this repo and submit a pull request.

---

## 📜 License

This project is licensed under the MIT License.

---

## 🙌 Acknowledgements

* Scikit-learn documentation
* UCI Machine Learning Repository

---

## ⭐ Support

If you found this project helpful, please give it a ⭐ on GitHub!
