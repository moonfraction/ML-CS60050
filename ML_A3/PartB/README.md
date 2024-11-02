# CS60050_Machine Learning: Programming Assignment 3 - Part B: K-Means Clustering - Anuran Calls Dataset (MFCCs)

## Project Code: PartB_ChandranshSingh_22CS30017


This repository focuses on clustering frog species based on their sound frequencies (MFCCs) using advanced clustering techniques, starting with K-Means. The project involves data preprocessing, exploratory data analysis (EDA), implementation of K-Means clustering, evaluation using various metrics, and comparison with other clustering algorithms.

## Note:
The Jupyter notebook (`PartB_ChandranshSingh_22CS30017.ipynb`) explains everything that has been done in the project, including the steps and techniques used.

## Features

1. **Data Preprocessing and Exploration:**
   - Exploratory Data Analysis (EDA) to check for missing values, feature distributions, and outliers.
   - Feature scaling using normalization or standardization.
   - Feature engineering to derive new features from MFCCs for improved clustering performance.

2. **Feature Correlation Analysis:**
   - Investigation of correlations between features to remove highly correlated features for better clustering results.

3. **K-Means Clustering:**
   - Implementation of the Elbow Method to determine the optimal number of clusters.
   - Evaluation of clustering quality using the Silhouette Score.
   - Comparison of different initialization methods for K-Means.

4. **Cluster Visualization:**
   - Application of dimensionality reduction techniques (PCA or t-SNE) for visualization purposes.
   - Visualization of clusters using 2D scatter plots.
   - Analysis of feature contributions to cluster separation.

5. **Cluster Evaluation Metrics:**
   - Calculation of additional metrics like Davies-Bouldin Index and Calinski-Harabasz Index to assess cluster quality.
   - Comparison of these metrics across different numbers of clusters.

6. **Comparison with Other Clustering Algorithms:**
   - Application of Agglomerative Hierarchical Clustering or DBSCAN.
   - Analysis of strengths and weaknesses of each algorithm in the context of this dataset.

## Dataset:

The Anuran Calls dataset (MFCCs) can be accessed on [Kaggle](https://www.kaggle.com/datasets/yasserhessein/anuran-calls-mfccs). This dataset includes 22 MFCC coefficients representing frog calls.

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