# Case-Study-How-Can-a-Wellness-Technology-Company-Play-It-Smart
Case Study done as part of Google's Data Analytics Professional Certificate


# Bellabeat Smart Device Data Analysis

## Project Overview

This project analyzes Fitabase smart device data to understand user activity, sleep, and fitness patterns. The analysis is intended to provide insights for Bellabeat's marketing team to inform product strategy and targeted campaigns for their health-focused smart devices.

### Bellabeat Products Focused

* **Bellabeat App**: Tracks health data including activity, sleep, stress, menstrual cycle, and mindfulness.
* **Leaf Tracker**: Wearable wellness tracker for activity, sleep, and stress.
* **Time Watch**: Smartwatch combining activity, sleep, and stress tracking.
* **Spring Water Bottle**: Tracks daily hydration.

## Dataset

### Source

* Fitabase Public Data (Kaggle): [Fitbit Fitness Tracker Data](https://www.kaggle.com/datasets/arashnic/fitbit)
* Dataset for 3/12/2016 - 4/11/2016 contains 11 CSV files:

  1. `dailyActivity_merged.csv`
  2. `heartrate_seconds_merged.csv`
  3. `hourlyCalories_merged.csv`
  4. `hourlyIntensities_merged.csv`
  5. `hourlySteps_merged.csv`
  6. `minuteCaloriesNarrow_merged.csv`
  7. `minuteIntensitiesNarrow_merged.csv`
  8. `minuteMETsNarrow_merged.csv`
  9. `minuteSleep_merged.csv`
  10. `minuteStepsNarrow_merged.csv`
  11. `weightLogInfo_merged.csv`

### Data Description

* Activity data: steps, calories, distance, and activity minutes.
* Heart rate: second-level heart rate data.
* Sleep: minute-level sleep data.
* Weight logs: weight and BMI tracking.
* Minute and hourly-level metrics for detailed user behavior analysis.

### Data Directory Structure

Place all CSV files in a folder, e.g. `Fitabase_3.12.16-4.11.16/`.

## Notebook Workflow

1. **Cell 1 - Imports & Setup**

   * Load libraries and define plotting settings.

2. **Cell 2 - Load & Clean Data**

   * Load all 11 CSVs without `parse_dates`.
   * Clean column names to lowercase with underscores.
   * Convert datetime columns safely if they exist.

3. **Cell 3 - Daily Summary**

   * Aggregate daily activity and sleep.
   * Add weekday column.

4. **Cell 4 - Exploratory Data Analysis**

   * Distribution of daily steps.
   * Average steps by weekday.

5. **Cell 5 - Correlation Analysis**

   * Compute correlation matrix for numeric daily metrics.

6. **Cell 6 - User Segmentation (K-Means)**

   * Cluster users based on average steps, calories, and sleep.

7. **Cell 7 - Retention Analysis**

   * Number of days recorded per user.
   * Percent of users with >=7 days of data.

8. **Cell 8 - Minute-Level Heatmaps**

   * Hourly activity intensity patterns by day of week.

9. **Cell 9 - User Cluster Visualization**

   * Scatter plot of average steps vs sleep colored by cluster.

10. **Cell 10 - Insights & Recommendations**

    * Key findings from analysis.
    * Marketing recommendations for Bellabeat products.


