# CS60050_Machine Learning: Programming Assignment 3 Part A: Support Vector Machines (SVMs) and Kernel Methods on HIGGS Dataset

## Project Code: PartA_ChandranshSingh_22CS30017

This repository focuses on building and evaluating a Support Vector Machine (SVM) classifier to predict whether a particle collision event is classified as a signal (Higgs boson) or background. The project involves data preprocessing, feature engineering and selection, implementation of SVMs with different kernels, hyperparameter tuning, and performance evaluation.

## Note:
The Jupyter notebook (`PartA_ChandranshSingh_22CS30017.ipynb`) provides detailed documentation and code with explanations for each step.

## Features

1. **Data Preprocessing and Exploration:**
   - Conduct Exploratory Data Analysis (EDA) to understand feature distributions and identify anomalies.
   - Apply normalization or standardization to ensure optimal model performance.

2. **Feature Engineering and Selection:**
   - Perform feature engineering to create new features (e.g., polynomial features, interaction terms).
   - Use techniques like Recursive Feature Elimination (RFE) or SelectKBest for dimensionality reduction.

3. **Linear SVM Implementation:**
   - Implement an SVM with a linear kernel and evaluate it using cross-validation.
   - Report metrics such as accuracy, precision, recall, F1-score, and AUC-ROC.
   - Discuss strategies for handling large-scale datasets (e.g., Stochastic Gradient Descent, mini-batch learning).

4. **SVM with Polynomial, RBF, and Custom Kernels:**
   - Implement and compare SVMs with polynomial (degrees 2, 3, 4), RBF, and custom kernels (e.g., sigmoid, hybrid).
   - Tune the regularization parameter \( C \) for each kernel using Grid Search or Random Search.
   - Compare the classification metrics and computational efficiency of each kernel.

5. **Hyperparameter Tuning and Sensitivity Analysis:**
   - Optimize hyperparameters using advanced methods like Bayesian Optimization or Random Search.
   - Visualize the impact of different hyperparameters (e.g., \( C \), gamma, kernel degree) on performance using heatmaps and line plots.

6. **Analysis and Report:**
   - Summarize results from all kernel methods and hyperparameter tuning.
   - Compare kernel performances based on classification metrics and efficiency.
   - Use SHAP or LIME for model interpretability and feature importance analysis.

## Evaluation Metrics:

The performance of the SVM classifiers is assessed using the following metrics:

- Accuracy
- Precision
- Recall
- F1-Score
- AUC-ROC

## Dataset:

The HIGGS dataset contains 28 physics-derived features from particle collision events for binary classification (signal vs. background). The dataset can be accessed from [UCI HIGGS Dataset](https://www.kaggle.com/datasets/erikbiswas/higgs-uci-dataset).

## Usage:

1. Clone the repository to your local machine:

   ```bash
   git clone https://github.com/moonfraction/ML-CS60050.git
   cd ML-CS60050


<hr>

To find the environment requirements for a Jupyter Notebook (`.ipynb`) in Visual Studio Code (VS Code), you can follow these steps:

1. **Open the Jupyter Notebook in VS Code**:
   - Open VS Code.
   - Use the File Explorer to navigate to your `.ipynb` file and open it.

2. **Identify the Libraries Used**:
   - Look through the notebook cells to identify all the libraries and packages that are imported and used. Typically, these are found at the beginning of the notebook.

3. **Generate a `requirements.txt` File**:
   - You can manually create a `requirements.txt` file by listing all the identified libraries and their versions. Alternatively, you can use a tool to automate this process.

4. **Using `pipreqs` to Generate `requirements.txt`**:
   - `pipreqs` is a tool that can automatically generate a `requirements.txt` file based on the imports in your project.
   - Install `pipreqs` if you haven't already:
     ```sh
     pip install pipreqs
   - Navigate to the directory containing your Jupyter Notebook:
     ```sh
     cd path/to/your/notebook
     ```
   - Run `pipreqs` to generate the `requirements.txt` file:
     ```sh
     pipreqs .
   - This will create a `requirements.txt` file in the current directory with all the necessary packages.

5. **Using `pip freeze` to Generate `requirements.txt`**:
   - If you have a virtual environment set up and all the required packages installed, you can use `pip freeze` to generate the `requirements.txt` file:
     ```sh
     pip freeze > requirements.txt

   - This will list all the installed packages and their versions in the `requirements.txt` file.

6. **Review and Edit `requirements.txt`**:
   - Open the generated `requirements.txt` file in VS Code.
   - Review the file to ensure it includes all the necessary packages and their correct versions. You can manually add or remove packages as needed.

7. **Install the Requirements**:
   - To install the packages listed in the `requirements.txt` file in a new environment, use the following command:
     ```sh
     pip install -r requirements.txt

By following these steps, you can identify and document the environment requirements for your Jupyter Notebook in VS Code.