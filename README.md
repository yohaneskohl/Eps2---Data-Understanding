---

# **Eps2 - Data Understanding**

## **Table of Contents**
1. [Introduction](#introduction)
2. [Project Overview](#project-overview)
3. [Data Description](#data-description)
4. [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
5. [Data Cleaning](#data-cleaning)
6. [Results and Insights](#results-and-insights)
7. [How to Run](#how-to-run)
8. [Contributor](#contributor)

---

## **Introduction** <a name="introduction"></a>
This project is part of an individual Data Mining course assignment that focuses on understanding data structures and performing exploratory analysis. The Titanic dataset is used to demonstrate methods for analyzing and cleaning data to derive insights.

## **Project Overview** <a name="project-overview"></a>
In this project:
- I conducted exploratory data analysis (EDA) using statistical and visual methods.
- I cleaned the dataset by handling missing values and optimizing data for further analysis.
- I derived insights regarding factors that contributed to survival rates on the Titanic.

## **Data Description** <a name="data-description"></a>
The dataset used in this project is the Titanic dataset, which contains information about passengers aboard the Titanic, including demographics, class, and whether they survived or not.

| Column   | Description                  |
|----------|------------------------------|
| `PassengerId` | Unique ID of the passenger |
| `Survived` | Survival status (0 = No, 1 = Yes) |
| `Pclass` | Passenger class (1st, 2nd, 3rd) |
| `Name` | Name of the passenger |
| `Sex` | Gender of the passenger |
| `Age` | Age of the passenger |
| `SibSp` | Number of siblings/spouses aboard |
| `Parch` | Number of parents/children aboard |
| `Fare` | Passenger fare |
| `Embarked` | Port of embarkation (C, Q, S) |

## **Exploratory Data Analysis (EDA)** <a name="exploratory-data-analysis-eda"></a>
### **Statistical Approach**
I began by analyzing key statistics of the dataset using `describe()` to summarize distributions:
- **Passenger Age**: Ranges from 0.42 to 80 years with an average of ~29.7.
- **Survival Rate**: Only 38% of passengers survived the disaster.

### **Visual Approach**
Several visualizations were created to understand relationships:
- Survival rates by **Gender** and **Class**.
- Stacked bar charts to show the survival distribution across different embarkation points and age groups.

## **Data Cleaning** <a name="data-cleaning"></a>
Missing data was handled by:
1. Removing columns with excessive missing data (e.g., `Cabin`).
2. Imputing missing values for `Age` using the mean, and for `Embarked` using the mode.

After cleaning, all missing values in critical columns were addressed.

## **Results and Insights** <a name="results-and-insights"></a>
Key findings include:
- **Women and children** had a higher survival rate compared to men.
- **First-class** passengers had a significantly higher survival rate compared to third-class passengers.
- Passengers who embarked from **Cherbourg (C)** had a higher chance of survival.

## **How to Run** <a name="how-to-run"></a>
1. Clone the repository:
   ```bash
   git clone https://github.com/yohaneskohl/Eps2---Data-Understanding.git
   ```
2. Install the necessary libraries:
   ```bash
   pip install pandas numpy matplotlib seaborn
   ```
3. Run the analysis in Jupyter Notebook or Google Colab.

## **Contributor** <a name="contributor"></a>
- **Kevin Yohanes Wuryanto** - 21082010193

This project is part of an individual Data Mining assignment for the **Data Mining** course at UPN "Veteran" East Java, supervised by **Amalia Anjani Arifiyanti, S.Kom., M.Kom**.

---
