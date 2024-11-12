# Ch.-1-Foundation-on-Artificial-Intelligence
The provided code consists of two main sections: one for calculating the number of banknotes and coins needed based on a given input value (in Indonesian Rupiah), and the other for performing HR data analysis using Python's pandas and data visualization with matplotlib and seaborn. Here's a breakdown of each section:

# Project Overview
# **1.  Calculating Banknotes and Coins Needed (01_Kelompok_G_2.ipynb)**
This code prompts the user to input an amount in Rupiah (integer) and calculates how many banknotes and coins are needed to make up that amount.

**Details of calculate_allmoney Function:**

- Stores various currency denominations in a dictionary allmoney.
- Divides banknotes and coins into two separate lists: paper_money and coins.
- Calculates the total number of banknotes (total_paper_money) and coins (total_coins) required using integer division (//) and modulus (%).
- Saves any remaining balance that cannot be exchanged if the amount is not a multiple of available denominations.

**Input Validation:**

Checks if the input is negative or exceeds Rp 1,000,000,000, displaying an appropriate message.

**Output:**

Prints the quantity of each denomination, the total banknotes, the total coins, and any remaining balance that cannot be exchanged.

# **2.  HR Data Analysis & Visualization (01_Kelompok_G_3.ipynb)**
This code performs several analyses on HR data (HRDataset_v14.csv) and generates different data visualizations.

**Analyses Performed:**

1. Salary Analysis: Groups data by marital status and gender, then calculates the minimum, median, maximum, and average salary using the agg function.
2. Top Termination Reasons: Groups termination reasons and displays the top 5 reasons using groupby and sort_values.
3. Best Performance Recruiting Sources: Identifies recruiting sources with the highest "Exceeds" performance, using a filter on the PerformanceScore column.
4. Number of Managers per Department: Counts the number of unique managers in each department using nunique.
5. Termination Ratio by Gender: Uses value_counts(normalize=True) to get the termination ratio per gender.

**Visualizations Created:**

1. Scatter Plot of Salary vs EngagementSurvey by Termd status.
2. Bar Chart of Employee Termination by Department.
3. Pie Chart Showing Termination Percentage by Position.
4. Boxplot of Salary by MaritalDesc and Termd Status.
5. Pairplot for Salary, EngagementSurvey, EmpSatisfaction, and Absences by Termd status.

**Statistical Analysis:**

- Relationship Between Manager and Performance Score: Uses a Chi-Square test to assess any association between ManagerName and PerformanceScore.
- Recruitment Sources with Low Termination Ratio: Groups data by RecruitmentSource and identifies sources with the lowest termination counts.
