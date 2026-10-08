# Samed-Itprojects
# Data Science Fundamentals Assessment: Iris Dataset Analysis

## Description
This project applies core data science fundamentals to the classic Iris flower dataset. It covers Python programming, data cleaning, statistical analysis, and exploratory data analysis (EDA), and ends with a documented analysis report. The goal is to understand which flower measurements best distinguish the three iris species.

Completed as **Task 1** of the Data Science Consultant Internship.

## Dataset Information
| Property | Details |
|---|---|
| Name | Iris Dataset |
| Source | scikit-learn built-in datasets (originally from the UCI Machine Learning Repository) |
| Records | 150 observations (149 after removing 1 duplicate) |
| Features | Sepal length, sepal width, petal length, petal width (all in cm) |
| Target | Species: setosa, versicolor, virginica (50 samples each) |
| Missing values | None |

**Business context:** classifying a species from measurable features, similar to any problem where an item must be categorized from its attributes (e.g. quality grading, product categorization).

## Project Steps
1. **Understand the dataset:** examine columns, data types, structure, and class balance.
2. **Apply Python fundamentals:** use data structures, functions, loops, conditionals, Pandas, and NumPy.
3. **Clean the data:** check for missing values, duplicates, inconsistent labels, and incorrect data types; remove the duplicate record.
4. **Apply statistical concepts:** calculate mean, median, mode, standard deviation, variance, and correlations.
5. **Perform exploratory data analysis:** build histograms, box plots, a correlation heatmap, a scatter plot, and a bar chart.
6. **Prepare the analysis report:** document the methodology, data preparation, statistical results, visualizations, and conclusions.

## Key Findings
- Petal length and petal width are the most informative features: they have the highest variance and are very strongly correlated (r ≈ 0.96).
- Setosa forms a clearly separate cluster, while versicolor and virginica partially overlap.
- Sepal width has the lowest variance and weak negative correlations with the other features, making it the weakest single predictor.
- **Recommendation:** prioritize petal length and petal width for any classification rule or model.

## Tools & Libraries
- Python 3
- Pandas, NumPy
- Matplotlib, Seaborn
- scikit-learn (dataset loading only)
- Jupyter Notebook

## Repository Structure
```
├── Data_Science_Fundamentals_Iris.ipynb   # Full analysis code with explanations
├── Iris_Data_Analysis_Report.docx         # Written analysis report
└── README.md
```

## How to Run
1. Clone the repository:
```bash
   git clone https://github.com/SAMEDWORK/<your-repo-name>.git
```
2. Install the required libraries:
```bash
   pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```
3. Launch Jupyter and open the notebook:
```bash
   jupyter notebook Data_Science_Fundamentals_Iris.ipynb
```
4. Run all cells from top to bottom.

## Author
**Mohamed Samed**
GitHub: [SAMEDWORK](https://github.com/SAMEDWORK)
