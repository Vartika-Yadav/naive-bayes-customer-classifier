# Naïve Bayes Customer Classifier

This project demonstrates the implementation of a **Naïve Bayes classifier** using a sample customer dataset stored in a CSV file.  
The notebook shows how to load data, preprocess it, train the model, and evaluate its performance.

---

## Objectives

1. Load and inspect the dataset (`customers-100.csv`).
2. Preprocess data including encoding categorical variables.
3. Split dataset into **training** and **test sets** (80%-20% split).
4. Train a **Gaussian Naïve Bayes classifier**.
5. Evaluate model accuracy on the test set.
6. Predict new samples (optional).

---

## Dataset

The CSV file contains customer information with the following columns:

- Index
- Customer Id
- First Name
- Last Name
- Company
- City
- Country
- Phone 1
- Phone 2
- Email
- Subscription Date
- Website (used as target)

Example data:

| Index | Customer Id | First Name | Last Name | Company | City | Country | Phone 1 | Phone 2 | Email | Subscription Date | Website |
|-------|------------|------------|-----------|--------|------|--------|---------|---------|-------|-----------------|---------|
| 1     | DD37Cf93aecA6Dc | Sheryl | Baxter | Rasmussen Group | East Leonard | Chile | 229.077.5154 | 397.884.0519x718 | zunigavanessa@smith.info | 2020-08-24 | http://www.stephenson.com/ |

---

## Steps Performed

1. **Data Preprocessing**
   - Load CSV file using `pandas`
   - Inspect data (`.info()`, `.describe()`)
   - Encode categorical variables using `pd.get_dummies`
   - Align train and test features after encoding

2. **Train-Test Split**
   - 80% of data for training, 20% for testing using `train_test_split`

3. **Model Training**
   - Initialize `GaussianNB()` model
   - Fit the model on training data

4. **Evaluation**
   - Predict on test set
   - Calculate **accuracy** using `accuracy_score`

---

## Results

- Training set size: 80 samples
- Test set size: 20 samples
- **Accuracy:** 100%

> Note: Accuracy may vary slightly depending on preprocessing and dataset specifics.
