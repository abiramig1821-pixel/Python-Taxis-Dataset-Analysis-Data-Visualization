# Data Analytics (DA) - Python Taxis Dataset Analysis & Data Visualization 

## 📌 Project Overview

This project focuses on cleaning, analyzing, and visualizing taxi trip data. Taxi services generate massive amounts of data daily, which can be leveraged to understand human behavior, optimize operations, and predict pricing. However, raw trip logs often contain missing values and anomalies that make them difficult to interpret without proper processing.
As a Data Analyst, this repository demonstrates how to handle missing data, identify core trends, and generate comprehensive visualizations to gain actionable insights into fare distribution, trip distances, and customer payment behaviors using Python's Pandas, Matplotlib, and Seaborn libraries.

## 🛠️ Key Tasks & Workflow

- **Data Loading:** Importing the Seaborn built-in taxis dataset into a Pandas Data Frame.
  
- **Data Cleansing & Imputation:** Identifying missing (null) values and applying statistical strategies (like mode imputation for categorical data) to maintain data integrity.
  
- **Exploratory Data Analysis (EDA):** Generating statistical summaries (describe(), info(), shape) to understand the dataset's structure.
  
- **Data Visualization (Matplotlib & Pandas Plot):**
    - Line charts to plot continuous variables (e.g., average fares) over time.
    - Bar charts to evaluate categorical aggregates (e.g., total fares per pickup borough).
    - Pie charts to analyze the percentage share of a dataset (e.g., payment options).
    - Histograms to view data distribution and granularity (e.g., trip distances).
    - Box plots to pinpoint outliers and data spreads (e.g., tip amounts per borough).
      
- **Advanced Visualization (Seaborn):**
    - Count plots for quick categorical frequency checks.
    - Scatter plots with hue mapping to analyze multidimensional correlations.
    - Heatmaps for evaluating linear relationships using correlation matrices.
    - Pair plots for wide-scope exploratory data grids.
________________________________________
## 📊 Dataset Structure
The dataset contains 6,433 rows and 14 columns tracking taxi trips from February to April 2019

| Column Name | Data Type | Description |
| :--- | :--- | :--- |
| `pickup` | `datetime64[ns]` | Date and time when the meter was engaged |
| `dropoff` | `datetime64[ns]` | Date and time when the meter was disengaged |
| `passengers` | `int64` | Number of passengers in the vehicle |
| `distance` | `float64` | The elapsed trip distance in miles |
| `fare` | `float64` | The time-and-distance fare calculated by the meter |
| `tip` | `float64` | Tip amount automatically populated for credit card payments |
| `tolls` | `float64` | Total amount of all tolls paid in trip |
| `total` | `float64` | The total amount charged to passengers |
| `color` | `object` | Type of taxi (e.g., yellow, green) |
| `payment` | `object` | Payment method used (credit card, cash) |
| `pickup_zone` | `object` | TLC taxi zone where the meter was engaged |
| `dropoff_zone` | `object` | TLC taxi zone where the meter was disengaged |
| `pickup_borough` | `object` | Borough where the taxi meter was engaged |
| `dropoff_borough` | `object` | Borough where the taxi meter was disengaged |

________________________________________

## 📈 Insights Found From Visualizations

Based on the analysis conducted in the notebook, several important patterns emerged:

- **Borough Dynamics:** Manhattan dominates the taxi service industry, yielding the highest number of overall trips and making up the massive majority of the total fare revenue, followed by Queens and Brooklyn.

- **Fares & Distance Trends:** There is a strong positive correlation (0.92) between trip distance and base fare, which naturally dictates the overall total amount paid.

- **Toll Spending:** Longer trip distances display a moderate positive correlation with toll fees, indicating that long-distance commutes frequently require crossing bridges or turnpikes.

- **Customer Tipping Behavior:** Tipping shows a moderate correlation with the final fare amount, meaning passengers generally scale their tips relative to the total cost of the ride.

- **Passenger Loads:** The number of passengers per trip shows zero correlation with distance, fare, or total costs, proving that party size does not influence trip patterns or pricing structures.
________________________________________

## 🚀 Getting Started

**Prerequisites:**

Make sure you have Python installed along with the following libraries:

```python
pip install pandas numpy matplotlib seaborn
```

**Running the Notebook**

1.	Clone this repository:
2.	git clone https://github.com
3.	Navigate to the project directory and launch your Jupyter interface (or open directly in Google Colab).
4.	Run the notebook cells sequentially to view the data processing steps and output graphs.

## Author:
### Abirami Ganesan
