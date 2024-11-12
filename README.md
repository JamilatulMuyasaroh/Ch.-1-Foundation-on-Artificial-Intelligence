# Ch. 1 - Foundation on Artificial Intelligence

This project covers two main sections:
1. Calculating the number of banknotes and coins needed based on a given amount in Indonesian Rupiah.
2. Performing HR data analysis using Python's pandas and data visualization with matplotlib and seaborn.

## Project Overview

### 1. Banknote and Coin Calculator (01_Kelompok_G_2.ipynb)
This code allows users to input an amount in Rupiah and calculates the number of banknotes and coins required to represent that amount.

#### Key Function: `calculate_allmoney`

- **Denominations**: Stores available currency denominations in a dictionary (`allmoney`).
- **Division of Currency**: Separates denominations into `paper_money` (banknotes) and `coins`.
- **Calculation**: Determines the number of each denomination using integer division (`//`) and modulus (`%`).
- **Remaining Balance**: Displays any remaining balance that cannot be exchanged if the amount is not a multiple of available denominations.

#### Input Validation
- Ensures the input is positive and does not exceed Rp 1,000,000,000, displaying an appropriate message if the input is invalid.

#### Output
- Prints the quantity of each denomination, the total banknotes, total coins, and any remaining balance that cannot be exchanged.

---

### 2. HR Data Analysis & Visualization (01_Kelompok_G_3.ipynb)
This section performs various analyses on HR data (`HRDataset_v14.csv`) and generates different data visualizations.

#### Analyses Performed

1. **Salary Analysis**: Groups data by marital status and gender, then calculates the minimum, median, maximum, and average salary using the `agg` function.
2. **Top Termination Reasons**: Groups termination reasons and displays the top 5 reasons using `groupby` and `sort_values`.
3. **Best Performance Recruiting Sources**: Identifies recruiting sources with the highest "Exceeds" performance using a filter on the `PerformanceScore` column.
4. **Number of Managers per Department**: Counts the number of unique managers in each department using `nunique`.
5. **Termination Ratio by Gender**: Uses `value_counts(normalize=True)` to get the termination ratio per gender.

#### Visualizations Created

1. **Scatter Plot** of Salary vs EngagementSurvey by `Termd` status.
2. **Bar Chart** of Employee Termination by Department.
3. **Pie Chart** showing Termination Percentage by Position.
4. **Boxplot** of Salary by `MaritalDesc` and `Termd` Status.
5. **Pairplot** for Salary, EngagementSurvey, EmpSatisfaction, and Absences by `Termd` status.

#### Statistical Analysis

- **Relationship Between Manager and Performance Score**: Uses a Chi-Square test to assess any association between `ManagerName` and `PerformanceScore`.
- **Recruitment Sources with Low Termination Ratio**: Groups data by `RecruitmentSource` and identifies sources with the lowest termination counts.

---

## Running the Notebooks

To run each notebook:

1. Open **Google Colab** or a compatible Jupyter Notebook environment.
2. Upload the respective `.ipynb` notebook file (01_Kelompok_G_2.ipynb or 01_Kelompok_G_3.ipynb).
3. Follow the instructions within each notebook to install any necessary libraries, such as `pandas`, `matplotlib`, `seaborn`, and others.
4. Execute each cell in sequence to perform calculations or generate analyses and visualizations.
   
Each notebook provides hands-on experience with fundamental AI tasks and data analysis techniques, guiding users through calculations, data processing, and visualization practices relevant to AI and HR analytics.
