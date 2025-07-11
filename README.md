# Breast Cancer Classification Using Machine Learning Tools

## Project Overview
This project applies popular machine learning techniques to classify histological cell images for diagnosing malignant breast cancer. The goal is to help a pathology lab client implement a model that can:

- Detect malignant cancer with at least 95% probability when present
- Misclassify no more than 10% of healthy (benign) cases as malignant

Using a dataset of 300 hand-labelled samples, the project follows a best-practice ML workflow: data investigation, visualization, preprocessing, model training, optimization, evaluation, and interpretation.

## Dataset
- The dataset consists of 300 samples with features extracted from histological images.
- Features include measurements like mean radius, texture, perimeter, area, smoothness, compactness, concavity, symmetry, and fractal dimension.
- Labels indicate whether samples are benign or malignant.

## Data Source
The data is derived from a pathology lab’s new imaging process similar to the Wisconsin breast cancer dataset but with different acquisition and processing methods.

## Analysis Summary
- Data exploration involved descriptive statistics and visualization of feature distributions per class.
- Data was split into training, validation, and test sets maintaining class stratification.
- Baseline classifiers were tested, including SGD, KNN, Decision Tree, SVM, and optimized using grid search.
- Model performance was measured using balanced accuracy, recall, precision, AUC, F1, and F-beta scores.
- The top features identified for classification were worst concave points, worst perimeter, worst radius, and mean concave points.
- Decision boundaries for the top features were visualized.
- A second round of analysis excluded "worst" features to evaluate performance trade-offs for reduced computational expense.

## Project Structure
- `assignment2.csv`: Dataset file containing feature values and labels.
- Jupyter notebooks and scripts (not shown here) performing data loading, processing, visualization, training, and evaluation.
- Visualizations include histograms, ROC curves, confusion matrices, and decision boundary plots.

## How to Run the Code
1. Ensure Python ≥ 3.5 is installed with the required packages: `numpy`, `pandas`, `scikit-learn`, `matplotlib`, `seaborn`.
2. Load the dataset `assignment2.csv` into your working directory.
3. Run the Jupyter notebooks or Python scripts sequentially to execute data processing, training, and evaluation.
4. Modify hyperparameters and model selection as needed.
5. Review generated plots and evaluation metrics for model insights.

## Project Report
A detailed project report titled [Breast Cancer Classification Report.pdf](./Breast%20Cancer%20Classification%20Report.pdf) has been uploaded.  
Click the link to view full methodology, model development steps, results, and conclusions.

## Contact
For any questions or feedback, please reach out via:  
**Email:** chavanyukta@gmail.com  

---

*This project was completed as part of a machine learning practical assignment focused on medical image classification and model evaluation.*
