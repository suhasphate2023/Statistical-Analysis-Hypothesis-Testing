# Statistical Analysis and Hypothesis Testing in Python Week 3

## 📌 Project Overview

This project performs statistical analysis and hypothesis testing on a **Student Performance Dataset** using Python.

The main objective is to determine whether there is a statistically significant difference in **Math Scores** between students who **completed test preparation** and students who **did not complete test preparation**.

---

## 🎯 Objective

To apply statistical methods in Python and understand whether test preparation is associated with a difference in students' Math Scores.

---

## ❓ Research Question

**Is there a significant difference in the average Math Scores of students who completed test preparation and those who did not?**

---

## 🧪 Hypothesis

### Null Hypothesis (H₀)

There is **no significant difference** in the average Math Scores between students who completed test preparation and those who did not.

### Alternative Hypothesis (H₁)

There is a **significant difference** in the average Math Scores between students who completed test preparation and those who did not.

### Significance Level

The significance level used for the test is:

**α = 0.05**

---

## 📊 Dataset

The project uses the file:

`Original_data_with_more_rows.csv`

Important variables used in the analysis:

* **TestPrep** – indicates whether the student completed test preparation.
* **MathScore** – student's Math Score.

The dataset contains **30,641 observations**.

---

## 🔬 Statistical Test

An **Independent Samples t-test (Welch's t-test)** is used because the analysis compares the mean Math Scores of two independent groups.

The two groups are:

1. Students who completed test preparation
2. Students who did not complete test preparation

Welch's t-test is used without assuming that the two groups have equal variances.

---

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* SciPy
* Matplotlib
* Jupyter Notebook / Python Script
* GitHub

---

## 📁 Project Structure

```text
Week_3_GitHub_Project/
│
├── Dataset.csv/
│   └── Original_data_with_more_rows.csv
│
├── graphs/
│   ├── math_score_histogram.png
│   └── math_score_boxplot.png
│
├── Analysis.ipynb/
│   └── hypothesis_testing.py
│
├── report/
│   └── Week_3_Hypothesis_Testing_Report.docx
│
├── README.md

```

---

## 💻 Python Analysis

The Python program performs the following steps:

1. Imports the required Python libraries.
2. Loads the student dataset.
3. Cleans the `MathScore` and `TestPrep` variables.
4. Separates students into two test-preparation groups.
5. Calculates the sample size, mean, and standard deviation.
6. Performs an independent samples Welch's t-test.
7. Calculates the difference between group means.
8. Calculates a 95% confidence interval.
9. Creates a histogram of Math Scores.
10. Creates a boxplot comparing the two groups.
11. Makes the final hypothesis-testing decision.

---

## 📈 Visualizations

### Histogram

The histogram shows the distribution of Math Scores for students in the two test-preparation groups.

### Boxplot

The boxplot compares the Math Score distributions between students who completed test preparation and those who did not.

---

## 📌 Results

The Welch independent samples t-test produced:

* **t-statistic:** approximately `-25.51`
* **p-value:** approximately `1.89 × 10⁻¹⁴¹`
* **95% Confidence Interval:** approximately `[-4.95, -4.25]`

Since the p-value is much smaller than **0.05**, the null hypothesis is rejected.

---

## ✅ Conclusion

There is a **statistically significant difference** in Math Scores between students who completed test preparation and those who did not.

Therefore, the analysis provides strong statistical evidence that the two test-preparation groups have different average Math Scores.

---

## ▶️ How to Run the Project

### 1. Clone the repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
```

### 2. Open the project folder

```bash
cd Week_3_GitHub_Project
```

### 3. Install the required libraries

```bash
pip install -r requirements.txt
```

### 4. Run the Python program

```bash
python notebooks/hypothesis_testing.py
```

The program will perform the statistical analysis and display the graphs.

---

## 📚 Learning Outcomes

Through this project, we learn how to:

* Work with real-world datasets using Python.
* Perform data cleaning.
* Calculate descriptive statistics.
* Formulate null and alternative hypotheses.
* Perform an independent samples t-test.
* Interpret p-values.
* Calculate and interpret confidence intervals.
* Create statistical visualizations.
* Make data-based conclusions.
* Document statistical analysis in a GitHub repository.

---

## 👨‍🎓 Project

**Week 3 Task – Statistical Analysis and Hypothesis Testing in Python**

**Topic:** Student Performance and Test Preparation

**Analysis:** Independent Samples t-test
