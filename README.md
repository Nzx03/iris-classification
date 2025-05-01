# 🌸 Iris Flower Classification

This project performs classification on the famous Iris dataset using three machine learning models:

- Decision Tree Classifier  
- Random Forest Classifier  
- Naive Bayes Classifier (CategoricalNB)

The goal is to predict the species of an iris flower based on features such as sepal length, sepal width, petal length, and petal width.

---

## 📁 Dataset

The dataset used is `iris.csv`, which contains 150 rows and the following columns:

- `sepal_length`
- `sepal_width`
- `petal_length`
- `petal_width`
- `species` (Target Variable)

---

## 🧪 Preprocessing

- Checked for **null values** — none were found.  
- Visualized feature distributions using **boxplots** and **histograms**.  
- Verified **skewness** of features, particularly `sepal_width`, which was approximately symmetric.  
- **No standardization** was applied since models like Decision Tree, Random Forest, and Naive Bayes do not require it.  
- For:
  - **Decision Tree and Random Forest**, the target was one-hot encoded.
  - **Naive Bayes**, label encoding was used (as CategoricalNB expects integer-labeled targets and categorical features).

---

## 🧠 Models and Results

### 🎯 Decision Tree Classifier
- `max_depth = 3`
- **Accuracy**: 0.9667  
- **Precision**: 1.0  
- **Recall**: 0.9667  
- **F1 Score**: 0.9830  
✅ Saved as: `dtree.pkl`

---

### 🌲 Random Forest Classifier
- Default parameters  
- **Accuracy**: 1.0  
- **Precision**: 1.0  
- **Recall**: 1.0  
- **F1 Score**: 1.0  
✅ Saved as: `rf.pkl`

---

### 🐦 Naive Bayes Classifier (CategoricalNB)
- Using label-encoded target and features  
- **Accuracy**: 0.9333  
- **Precision**: 0.9556  
- **Recall**: 0.9333  
- **F1 Score**: 0.9333  
✅ Saved as: `model.pkl`

---

## 🧰 Dependencies

The required dependencies are listed in `requirements.txt`.

Install them using:

```bash
pip install -r requirements.txt
