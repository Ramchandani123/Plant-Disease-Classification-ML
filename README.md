
# 🌿 Plant Pathology - Traditional ML Project (Kaggle FGVC7)

This project classifies leaf images into four categories: `healthy`, `rust`, `scab`, and `multiple_diseases` using traditional machine learning models **without deep learning** or transfer learning.

## 📁 Dataset
Dataset is sourced from the [Kaggle Plant Pathology 2020 - FGVC7](https://www.kaggle.com/c/plant-pathology-2020-fgvc7) competition.

- Training: `train.csv` + `images/`
- Testing: `test.csv`
- Sample Submission: `sample_submission.csv`

## 🧠 Methodology

### 🔍 Feature Engineering
- Images resized to 64x64 pixels
- Converted to grayscale
- Flattened to 1D feature vectors
- Optionally extracted handcrafted texture features (e.g., LBP)

### ⚙️ Models Used
- `Random Forest Classifier` 🌲
- `Bagging Classifier` (with Decision Tree base)
- `XGBoost Classifier` ⚡

### 🧪 Evaluation
- Train/test split with stratified sampling (80/20)
- Evaluation metrics: accuracy, confusion matrix, classification report

## 📈 Results

| Model       | Accuracy | Notes                          |
|-------------|----------|--------------------------------|
| RandomForest| ~44%     | Base model                    |
| Bagging     | ~48%     | Slight improvement with variance reduction |
| Boosting    | ~51%     | Best performance with XGBoost  |

## 📊 Visualizations
- Class distribution bar chart
- Sample leaf images from each class
- Confusion matrices
- ROC curves

## 📦 Output
- `submission.csv` file with predicted probabilities for Kaggle submission.

## 📝 How to Run

1. Place all dataset files in `Plant patho/` directory.
2. Run the notebook `Plant_FINAL_PROJECT.ipynb` sequentially.
3. Upload the generated `submission.csv` to Kaggle.

---

**Made with ❤️ by Himanshu Ramchandani**
