# Day 2 report 
1. Dataset name 
-> Titanic-Dataset.csv

2. Number of Rows
->891

3. Number of Columns
->12

4. Total missing values
->866

5. Duplicate Rows
-> 0

6. Numerical Columns
-> ['PassengerId', 'Survived', 'Pclass', 'Age', 'SibSp', 'Parch', 'Fare']

7. Categorical Columns
-> ['Name', 'Sex', 'Ticket', 'Cabin', 'Embarked']

8. Boolean Columns
-> []

9. Initial Observations
-> 1. The dataset contains passenger information such as age, gender, ticket, class, and fare.
   2. Some columns contain missing values, especially Age, Cabin, and Embarked.
   3. The dataset contains both numerical and categorical features.
   4. No duplicate rows were found in the dataset.
   5. The dataset can be used for predicting whether a passenger survived based on different features.

# Day 3 report
# Day 3 Report

## Project Name
Titanic Data Cleaning Project

## Objective
The objective of Day 3 was to clean the Titanic dataset by handling missing values and preparing the data for further analysis and visualization.

## Tasks Performed

### 1. Checked Missing Values
- Used `df.isnull().sum()` to identify missing values in each column.
- Calculated the percentage of missing values.

### 2. Visualized Missing Values
- Generated a heatmap using Seaborn to visualize missing data.
- Observed that the Cabin column contained a large number of missing values.

### 3. Removed Unnecessary Column
- Removed the `Cabin` column because it contained approximately 77% missing values, making it unsuitable for analysis.

### 4. Filled Missing Values
- Filled missing values in the `Age` column using the median value.
- Filled missing values in the `Embarked` column using the mode (most frequent value).

### 5. Verified Data Cleaning
- Checked the dataset again to ensure that all missing values were handled successfully.

### 6. Saved the Cleaned Dataset
- Saved the cleaned dataset as `cleaned_titanic.csv`.

## Libraries Used
- Pandas
- NumPy
- Matplotlib
- Seaborn

## Key Observations
- The `Cabin` column had a significant number of missing values and was removed.
- The `Age` column contained several missing values which were replaced with the median.
- The `Embarked` column contained only a few missing values which were replaced using the mode.
- After cleaning, the dataset contained no missing values.

## Learning Outcomes
- Learned how to identify missing values.
- Understood different techniques to handle missing data.
- Learned when to drop a column instead of filling missing values.
- Successfully prepared a clean dataset for further analysis.

## Conclusion
The dataset was successfully cleaned and saved. It is now ready for data visualization and exploratory data analysis.


# Day 4 Report

## Project Name
Titanic Data Visualization Project

## Objective
The objective of Day 4 was to visualize the cleaned Titanic dataset and understand the distribution of passengers, survival patterns, and important characteristics using different charts.

## Tasks Performed

### 1. Loaded the Cleaned Dataset
- Loaded `cleaned_titanic.csv` into a Pandas DataFrame.

### 2. Created Visualizations

#### Age Distribution
- Created a histogram with a KDE curve.
- Saved as `age_distribution.png`.

#### Survival Count
- Created a count plot showing the number of passengers who survived and did not survive.
- Saved as `survival_count.png`.

#### Gender Distribution
- Created a count plot showing the number of male and female passengers.
- Saved as `gender_distribution.png`.

#### Survival by Gender
- Compared survival counts of male and female passengers.
- Saved as `survival_by_gender.png`.

#### Passenger Class Distribution
- Visualized the number of passengers in each class.
- Saved as `class_distribution.png`.

#### Fare Distribution
- Created a histogram showing the distribution of ticket fares.
- Saved as `fare_distribution.png`.

## Libraries Used
- Pandas
- Matplotlib
- Seaborn

## Key Observations
- Most passengers were between 20 and 40 years old.
- More passengers did not survive than survived.
- The dataset contains more male passengers than female passengers.
- Female passengers had a higher survival rate than male passengers.
- Third-class passengers represented the largest group.
- Ticket fare distribution is positively skewed because a small number of passengers paid very high fares.

## Learning Outcomes
- Learned how to create histograms and count plots.
- Learned how to compare categories using grouped count plots.
- Understood the importance of data visualization in exploratory data analysis.
- Learned how to save graphs as PNG files for reports and presentations.

## Conclusion
Data visualization provided valuable insights into the Titanic dataset and helped identify important survival trends and passenger characteristics. These visualizations will support further exploratory data analysis and machine learning tasks.

# Day 5 Report
## Objective 
Perform advanced visualization and detect outliers in the cleaned Titanic Dataset

## Tasks Performed
- Created a correlation heatmap.
- Generated boxplots for Fare and Age.
- Created a pairplot for numerical features.
- Detected outliers using the IQR method.

## Key Observations
- Fare contains several high-value outliers.
- Age has a few outliers but fewer than Fare.
- Most numerical variables have weak correlations.
- Pairplot helps visualize relationships between variables and survival.

## Learning Outcomes
- Learned to use heatmaps for correlation analysis.
- Learned to identify outliers using boxplots.
- Learned the IQR method for outlier detection.
- Understood how pairplots reveal relationships between multiple variables.

## Conclusion
Advanced visualizations provided deeper insights into the Titanic dataset and highlighted outliers that should be considered before building machine learning models.