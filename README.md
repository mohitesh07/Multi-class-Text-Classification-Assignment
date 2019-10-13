# Multi-class-Text-Classification-Assignment

![Version Details](https://img.shields.io/badge/version-1.0-brightgreen.svg)
![Download Details](https://img.shields.io/github/downloads/mohitesh07/Multi-class-Text-Classification-Assignment/total.svg)
![GitHub contributors](https://img.shields.io/github/contributors/mohitesh07/Multi-class-Text-Classification-Assignment.svg)

Classifies the job description based on the section text.
```
Label Details:
0 → 'Desired Qualifications'
1 → 'About Us'
2 → 'Role Title'
3 → 'Description'
4 → 'Location'
5 → 'Responsibilities',
6 → 'Required Qualifications'
7 → 'Benefits'
8 → 'Education'
```

Dataset
```
Confidential
```

Dependencies
```
python3
sk-learn
numpy
pandas
seaborn
matplotlib.pyplot
warnings
```

### Usage Instructions

```
Put two .csv files 'train.csv' and 'valid.csv' in the directory of main.ipynb
Restart Kernel and Run all cells
```

### Approach

```
Step 1. Import neccesary modules and methods.
Step 2. Read 'train.csv' and store into pandas dataframe 
Step 3. Train a TfidfVectorizer() model to transform words to numbers by calculating the inverse document frequency
Step 4. Compare accuracy of LinearSVC, LogisticRegression, MultinomialNB, RandomForestClassifier
Step 5. Divide the training dataset to train and test parts with 33% test
Step 6. SVM shows the best accuracy by far here. So train SVM
Step 7. Show the Confusion matrix on test set
Step 8. Read and store 'valid.csv' into a dataframe
Step 9. Convert the features of valid.csv to numbers with TfidfVectorizer() model made earlier
Step 10. Predict the result using the input of features on the earliear SVM model
Step 11. Display the Precision, Recall, f1-score values.
```
