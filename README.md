# Exploratory Data Analysis (EDA) using Seaborn Datasets

##  Project Overview

This project demonstrates **Exploratory Data Analysis (EDA)** using popular built-in datasets from the **Seaborn** library. The main focus is on understanding data structure, handling missing values, and visualizing relationships between numerical and categorical variables using Python visualization libraries.

The notebook/script explores two datasets:

* **Tips Dataset** – for basic data inspection and descriptive statistics
* **Titanic Dataset** – for missing value analysis and extensive univariate & bivariate visualizations

---

##  Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Jupyter Notebook / Google Colab

---

##  Datasets Used

### 1. Tips Dataset

* Records: 244
* No missing values in key numerical columns (`total_bill`, `tip`, `size`)
* Used for:

  * Shape and structure analysis
  * Descriptive statistics
  * Numerical and categorical feature understanding

### 2. Titanic Dataset

* Records: 891
* Contains significant missing values
* Used for:

  * Missing value percentage analysis
  * Data loss calculation
  * Strategy selection for null value treatment
  * Visualization-driven insights

---

##  Key Analysis Steps

### 1. Data Understanding

* `.shape`, `.columns`, `.info()`, `.describe()`
* Separation of numerical and categorical variables

### 2. Missing Value Analysis

* Identification of missing values using:

  ```python
  df.isna().sum()
  ```
* Percentage calculation of missing data
* Data loss estimation after dropping null values

### 3. Missing Value Handling Strategy

* **Remove columns** with more than 20% missing values (e.g., `deck` ~77%)
* **Impute missing values**:

  * Numerical → Median
  * Categorical → Mode

---

##  Data Visualization

### Univariate Analysis

* Histograms for numerical features (`age`, `fare`, `pclass`, etc.)
* Count plots for categorical features (`sex`, `class`, `embarked`, etc.)

### Bivariate Analysis

* Numerical vs categorical comparisons using `hue`
* Survival analysis based on:

  * Gender
  * Passenger class
  * Embark location
  * Family status

### Visualization Libraries

* `sns.histplot()`
* `sns.countplot()`
* `matplotlib.pyplot`

---

##  Key Insights

* Females had a higher survival rate than males
* First-class passengers had better survival chances
* Fare distribution is right-skewed
* Passengers traveling alone had lower survival probability
* Missing values significantly impact dataset size if dropped blindly

---

##  How to Run the Project

1. Install dependencies:

```bash
pip install pandas numpy matplotlib seaborn
```

2. Run the script or notebook:

```bash
python 18th_dec.py
```

*or open in Jupyter / Colab*

---

##  Learning Outcomes

* Practical EDA workflow
* Handling missing data effectively
* Visual storytelling using data
* Understanding real-world datasets

---

# Author

Created for learning and practice in **Data Analysis & Visualization using Python**.

---

##  License

This project is for **educational purposes only**.
