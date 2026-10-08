# Hands-On Data Lab Implementation: Titanic Dataset

## Description
This project is a hands-on data lab that walks through a complete Python data science workflow on the Titanic passenger dataset. It covers environment setup, data exploration, manipulation, cleaning, visualization, and basic analysis, using Pandas, NumPy, Matplotlib, and Seaborn in a Jupyter Notebook. The goal is to understand which factors influenced passenger survival.

Completed as **Task 2** of the Data Science Consultant Internship.

## Dataset Information
| Property | Details |
|---|---|
| Name | Titanic Dataset |
| Source | Seaborn built-in datasets (`sns.load_dataset('titanic')`) |
| Records | 891 passengers |
| Columns | 15 (age, sex, pclass, fare, sibsp, parch, embarked, class, who, deck, alive, and more) |
| Target | `survived` (0 = did not survive, 1 = survived) |
| Missing values | `deck` (most rows), `age`, and a few `embarked` / `embark_town` entries |

## Project Steps
1. **Set up the environment:** import Pandas, NumPy, Matplotlib, and Seaborn, and configure display and plot settings.
2. **Import and explore the data:** load the dataset and inspect it with `.head()`, `.info()`, and `.describe()`, then check for missing values.
3. **Manipulate the data:** filter (first-class female passengers), sort by fare, group survival rate by class and gender, and engineer new columns (`age_group`, `family_size`).
4. **Clean the data:** impute missing `age` with the median, drop the sparse `deck` column, fill missing `embarked` values with the mode, remove duplicates, and convert categorical columns to the correct data type.
5. **Visualize the data:** bar chart (survival by gender), histogram (age distribution), box plot (fare by class), and correlation heatmap.
6. **Analyze and summarize:** compute survival statistics and document the key insights.

## Key Findings
- Gender was the strongest predictor of survival: women survived at a far higher rate than men.
- Passenger class had a clear effect: 1st class had the highest survival rate and 3rd class the lowest.
- Fare and class are closely related (higher class, higher fare).
- Small families (2 to 4 members) tended to survive more often than passengers travelling alone or in very large families.

## Tools & Libraries
- Python 3
- Pandas, NumPy
- Matplotlib, Seaborn
- Jupyter Notebook

## Repository Structure
```
├── Titanic_Data_Lab.ipynb          # Full lab code with explanations
├── Titanic_Data_Lab_Report.docx    # Written lab report
└── README.md
```

## How to Run
1. Clone the repository:
```bash
   git clone https://github.com/SAMEDWORK/samed-itsprojects.git
```
2. Install the required libraries:
```bash
   pip install pandas numpy matplotlib seaborn jupyter
```
3. Launch Jupyter and open the notebook:
```bash
   jupyter notebook Titanic_Data_Lab.ipynb
```
4. Run all cells from top to bottom. An internet connection is needed the first time, because Seaborn downloads the Titanic dataset.

## Author
**Mohamed Samed**
GitHub: [SAMEDWORK](https://github.com/SAMEDWORK)