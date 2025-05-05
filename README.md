# 🎯 Sonar Mine Detection Using Logistic Regression

This project uses machine learning (Logistic Regression) to classify sonar signals as either **Rock** or **Mine** based on their frequency response data. The dataset consists of numerical features, each representing the sonar signal's strength at different frequencies.

---

## 📂 Dataset

- **Source**: UCI Machine Learning Repository – Sonar Dataset
- **Features**: 60 continuous features, each representing sonar signal strength at a different frequency.
- **Target**: The target variable is:
  - `R` = Rock
  - `M` = Mine

You can download the dataset from [Sonar Dataset](https://drive.google.com/file/d/1pQxtljlNVh0DHYg-Ye7dtpDTlFceHVfa/view?usp=sharing) and place it in the `data/` folder.

---

## 🧠 Model Used

- **Logistic Regression**: Chosen for its simplicity and effectiveness in binary classification tasks.

---

## 📊 Accuracy

- **Training accuracy**: ~`<0.8342245989304813>`  
- **Test accuracy**: ~`<0.7619047619047619>`

---

## 🧪 How to Use

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/sonar-mine-predictor.git
   cd sonar-mine-predictor

### 🧩 Dependencies (REQUIREMENTS)
To run this project, you need to install the following Python libraries:

numpy

pandas

scikit-learn


### 🧮 Code Explanation
Data Preprocessing
Loading Dataset: We load the dataset using pandas.read_csv.

Feature and Target Variables:

Features (X) are all columns except the last one (label).

Target (Y) is the label column, which is the last column (60).

Model Training
Train-Test Split: We split the data into training (90%) and testing (10%) sets using train_test_split from sklearn.

Model: We use Logistic Regression from sklearn.linear_model to train the model on the training dataset.

Model Evaluation
We evaluate the accuracy on both the training and test datasets using accuracy_score from sklearn.metrics.

Making Predictions
A sample input data tuple (input_data) is reshaped and passed to the model for prediction.

Based on the model's prediction:

R: The object is classified as a Rock.

M: The object is classified as a Mine.

   
