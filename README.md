# EDA-Task5
# Titanic Dataset - Exploratory Data Analysis (EDA)

## Objective
Perform Exploratory Data Analysis (EDA) on the Titanic dataset to uncover hidden insights, trends, and patterns that influenced passenger survival.

## Dataset
- **Source**: [Kaggle Titanic Dataset](https://www.kaggle.com/c/titanic/data)
- **Features**: PassengerId, Survived, Pclass, Name, Sex, Age, SibSp, Parch, Ticket, Fare, Cabin, Embarked

## 🛠 Tools Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Google Colab

## EDA Process

### 1. **Data Loading & Exploration**
- Used `.info()`, `.describe()`, and `.value_counts()` to understand data types, missing values, and unique distributions.

### 2. **Data Cleaning**
- Handled missing values in `Age` (filled with median), `Embarked` (filled with mode).
- Dropped `Cabin` due to excessive null values.
- Removed irrelevant columns: `PassengerId`, `Name`, `Ticket`.

### 3. **Univariate Analysis**
- Analyzed individual features like `Survived`, `Sex`, `Pclass`, and `Age` using countplots and histograms.

### 4. **Bivariate & Multivariate Analysis**
- Explored relationships between `Survived` and:
  - `Sex`, `Pclass`, `Age`, `Fare`, `Embarked`
- Used `countplot`, `boxplot`, `heatmap`, and `pairplot` for visual representation.

### 5. **Survival Summary by Group**
- Created a table showing number of **Survived** and **Dead** passengers based on **Sex** and **Pclass**.

## Key Insights

| Sex    | Pclass | Survived | Dead |
|--------|--------|----------|------|
| Female | 1      | 91       | 3    |
| Female | 2      | 70       | 6    |
| Female | 3      | 72       | 72   |
| Male   | 1      | 45       | 77   |
| Male   | 2      | 17       | 91   |
| Male   | 3      | 47       | 300  |

- Females had higher survival rates, especially in higher classes.
- 1st class passengers had better chances of survival.
- Males in 3rd class had the lowest survival rate.
