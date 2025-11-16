This notebook focuses on exploring the Titanic dataset in detail and preparing it for machine learning. This includes visualizations, summary statistics, and correlation analysis to better understand the data.

1. Loaded the dataset
I imported the Titanic CSV file using pandas and looked at the first few rows. This helped me understand the shape of the dataset and spot any obvious issues.

2. Explored the data
To get a clearer picture of what I was working with, I checked:
Column types
Missing values
Basic descriptive statistics
This allowed me to identify which features needed cleaning and transformations.

3. Handled missing values
Some columns had null values, so I filled them using common approaches like mean or median imputation. After this step, I confirmed that the missing values were fixed using df.info().

4. Removed unnecessary or high-cardinality columns
Columns that didn’t contribute much to modeling (like PassengerId, Name, Ticket, etc.) were dropped. This makes the dataset simpler and easier to use for ML algorithms.

5. Encoded categorical variables
Columns such as Sex and Embarked were converted into numerical features using one-hot encoding. I used get_dummies with drop_first=True to avoid redundancy.

6. Scaled the numerical columns
I applied standardization to the numerical features so that all values were on a similar scale. This step helps machine learning models perform better.

7. Visualized outliers
I plotted boxplots (especially for the Fare column) to identify extreme values. Based on the visualization, outliers were removed to keep the dataset more stable.

8. Summary statistics
I calculated:
Descriptive statistics for numeric columns
Value counts for categorical columns (like Embarked)
These insights helped me understand the distribution of different variables.

9. Visualized distributions
Using histograms, I plotted all numeric features to see how they were spread. This helped identify skewness and unusual patterns in the data.

10. Correlation Analysis
I created a correlation matrix and heatmap to check how different numerical attributes relate to the Survived column. This gives an idea of which features might be useful for modeling.
