# Text Classification Battle: Compare, Analyze and Defend

## Information Retrieval – CLA-2 Project

### Project Overview
This project compares four machine learning algorithms for text classification using the **SMS Spam Collection dataset**. The objective is to identify spam and legitimate (ham) SMS messages and evaluate the performance of different classification algorithms using the same dataset and evaluation procedure.

### Objectives
- Classify SMS messages as spam or ham.
- Apply TF-IDF vectorization to convert text into numerical features.
- Compare four machine learning algorithms using evaluation metrics.
- Analyze confusion matrices and classification performance.
- Perform a what-if experiment to study the effect of different K values in K-Nearest Neighbors (KNN).
- Recommend the most suitable model based on experimental results.

### Dataset
**Dataset:** SMS Spam Collection

The dataset contains labeled SMS messages with two columns:
- `label` – Message category (`ham` or `spam`)
- `message` – SMS text content

**Dataset summary:**
- Total messages: 5,169
- Ham messages: 4,516
- Spam messages: 653

The dataset is divided into 80% training data and 20% testing data using stratified sampling to preserve the class distribution.

### Algorithms Compared
1. **Decision Tree** – Classifies messages using decision rules.
2. **K-Nearest Neighbors (KNN)** – Predicts message categories based on the nearest text vectors.
3. **Support Vector Machine (SVM)** – Separates message categories using a linear decision boundary.
4. **Naive Bayes** – Uses probability-based classification for text data.

### Methodology
1. Load and inspect the SMS Spam Collection dataset.
2. Check the distribution of spam and ham messages.
3. Split the dataset into training and testing sets.
4. Apply TF-IDF vectorization with a maximum of 10,000 features and unigram/bigram features.
5. Train the four classification algorithms.
6. Evaluate each model on the same test dataset.
7. Compare the evaluation metrics and confusion matrices.
8. Perform a KNN what-if experiment using different values of K.
9. Visualize the results and identify the recommended model.

### Evaluation Metrics
The models are evaluated using:
- Accuracy
- Spam Precision
- Spam Recall
- Spam F1-score
- Confusion Matrix

Spam precision measures how many messages predicted as spam are actually spam. Spam recall measures how many actual spam messages are detected. The F1-score balances precision and recall.

### What-If Analysis
The KNN experiment tests the following values of K:

`K = 1, 3, 5, 7, 11`

The results are compared to understand how changing the number of neighbors affects spam detection and overall classification performance.

### Results and Visualizations
The following output files are included in this repository:

- `algorithm_comparison.csv` – Performance comparison of all four algorithms.
- `knn_what_if_results.csv` – KNN experiment results for different K values.
- `algorithm_comparison.png` – Visual comparison of model performance.
- `four_confusion_matrices.png` – Confusion matrices for the four classifiers.
- `knn_what_if_analysis.png` – Visualization of the KNN what-if experiment.

**Preliminary finding:** SVM achieved the highest spam F1-score in the experiment. Refer to the comparison CSV and graphs for the detailed metric values.

### Conclusion
This project demonstrates how machine learning algorithms can be applied to SMS spam detection using TF-IDF features. Comparing the models using the same train-test split and evaluation metrics provides a consistent basis for selecting a classifier. The KNN what-if experiment further illustrates how model parameters can influence classification performance.

### Tools and Technologies
- Python
- Google Colab
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- TF-IDF Vectorization
- GitHub

### How to Run
1. Open `IR_CLA2_Text_Classification.ipynb` in Google Colab.
2. Run the notebook cells in order.
3. Ensure the dataset is available to the notebook.
4. Review the generated comparison tables, confusion matrices, and KNN analysis.

### Project Deliverables
- Jupyter Notebook
- Algorithm comparison CSV
- KNN what-if results CSV
- Model comparison graph
- Four confusion matrices
- KNN what-if analysis graph

---

**Academic Project:** Information Retrieval – CLA-2  
**Topic:** Text Classification Battle — Compare, Analyze and Defend
