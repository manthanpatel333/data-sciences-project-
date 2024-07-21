
Introduction
This project involves preprocessing and transforming a dataset (vTargetMailCustomer.csv) to predict future bike buyers. The process includes selecting relevant features, handling missing values, performing sampling, calculating statistics, identifying data dispersion, detecting outliers, and normalizing data. The final dataset is stored in a new file named `vTargetBuyers.csv`.

Project Steps

Lab 1: Data Preparation
1. Install SQL Server Management Studio (SSMS):
   - Install SSMS to manage the database and import CSV files.

2. Create Database and Import CSV:
   - Create a database using SSMS.
   - Import the `vTargetMailCustomer.csv` file into the database.
   - Execute a query to retrieve data from the CSV file.

3. Create New View and Export CSV:
   - Create a new view to filter and select relevant features.
   - Export the filtered data as `vTargetBuyers.csv` for further analysis using Python in Jupyter Notebook (within Visual Studio Code).

Feature Selection
1. Select Relevant Features:
   - Examine each attribute in the dataset to select features that impact predicting bike buyers.
   - Include `CustomerKey` and `BikeBuyer` (class attribute) in the final dataset.
   - Remove unnecessary attributes.

2. Determine Attribute Properties:
   - Identify the type of each attribute (Nominal, Ordinal, Interval, Ratio).
   - Determine the data type (Discrete, Continuous).

| Attribute           | Type              | Data Type       |
|---------------------|-------------------|-----------------|
| CustomerKey         | Continuous        | Continuous      |
| MaritalStatus       | Binary            | Discrete        |
| Gender              | Binary            | Discrete        |
| YearlyIncome        | Continuous        | Continuous      |
| TotalChildren       | Discrete          | Discrete        |
| NumberChildrenAtHome| Discrete          | Discrete        |
| HouseOwnerFlag      | Binary            | Discrete        |
| NumberCarsOwned     | Discrete          | Discrete        |
| DateFirstPurchase   | Discrete          | Discrete        |
| CommuteDistance     | Discrete          | Discrete        |
| Region              | Nominal           | Discrete        |
| Age                 | Discrete          | Discrete        |

Data Preprocessing and Transformation
1. Import Libraries and Load Data:
   - Import necessary libraries (pandas, numpy, etc.).
   - Load `vTargetBuyers.csv` into a variable for processing.

2. Handling Null Values:
   - Identify and replace null values using appropriate techniques.

3. Perform Sampling:
   - Perform random sampling and bootstrap sampling with replacement to understand the data.

4. Calculate Statistics:
   - Compute mean, variance, and standard deviation for ordinal numeric attributes to understand data distribution and identify outliers.

5. Identify Data Dispersion:
   - Use visualization methods (Box plot, Histogram, z-score) to identify data dispersion.

Data Visualization
1. Box Plot Analysis:
   - Analyze data distribution using box plots to identify potential customers based on age, income, number of children, etc.

2. Histogram Analysis:
   - Create histograms to visualize the distribution of attributes like yearly income, number of cars owned, and age.

3. Outlier Detection:
   - Identify and replace outliers using the 1.5IQR method.

4. Discretization:
   - Perform binning/histogram on continuous features to create groups for better understanding.

5. Quartile Analysis:
   - Calculate Q1, median, and Q3 of grouped data to understand data ranges and identify outliers.

Data Transformation
1. Binarization:
   - Convert features to binary values (0 and 1) for machine learning compatibility.

2. Normalization/Standardization:
   - Normalize age and yearly income using z-score to facilitate comparison between similar datasets.

Conclusion
The project involved thorough preprocessing and transformation of the dataset to prepare it for predictive modeling. By selecting relevant features, handling missing values, performing sampling, calculating statistics, identifying outliers, and normalizing data, we ensured the dataset is clean and ready for further analysis and machine learning tasks.

Requirements
- SQL Server Management Studio (SSMS)
- Visual Studio Code
- Python (Jupyter Notebook)
- Libraries: pandas, numpy, matplotlib

Files
- `vTargetMailCustomer.csv`: Original dataset.
- `vTargetBuyers.csv`: Processed dataset with selected features.

Author
Manthan Patel

Date
April 2024
