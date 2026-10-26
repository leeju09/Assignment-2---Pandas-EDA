# Pandas Exploratory Data Analysis — Tips Dataset

An exploratory data analysis (EDA) of the classic **Tips dataset** using Python and Pandas. This project walks through dataset inspection, descriptive statistics, data quality assessment, and insight generation for a real-world restaurant tipping dataset.

---

## Table of Contents

- Overview
- Dataset
- Objectives
- Project Structure
- Getting Started
- Analysis Walkthrough
- Key Findings
- Data Quality Report
- Technologies Used
- How to Run
- Author
- Acknowledgements

---

## Overview

This project performs a full exploratory data analysis on the **Tips dataset**, which contains information about 244 restaurant bills — including total bill amount, tip amount, customer demographics, and dining context.

The goal is to demonstrate core Pandas skills:

- Loading and inspecting a real-world dataset
- Understanding data structure, shape, and types
- Detecting and analyzing missing data
- Computing descriptive statistics for numerical and categorical variables
- Generating meaningful insights before any modeling work

The analysis is split into four parts, each aligned with the assignment rubric:

| Part | Focus | Points |
|---|---|---|
| Part 1 | Initial Data Exploration | 8 |
| Part 2 | Descriptive Statistics | 10 |
| Part 3 | Data Quality Assessment | 4 |
| Part 4 | Summary and Insights | 3 |
| **Total** | | **25** |

---

## Dataset

**Source:** [Seaborn Tips Dataset](https://raw.githubusercontent.com/mwaskom/seaborn-data/master/tips.csv)

The dataset contains **244 rows** and **7 columns**:

| Column | Type | Description |
|---|---|---|
| `total_bill` | float | Total bill amount (USD) |
| `tip` | float | Tip amount (USD) |
| `sex` | object | Customer sex (Male / Female) |
| `smoker` | object | Smoking status (Yes / No) |
| `day` | object | Day of week (Fri, Sat, Sun, Thur) |
| `time` | object | Meal time (Lunch / Dinner) |
| `size` | int | Party size (number of people) |

---

## Objectives

By completing this analysis, the project demonstrates the ability to:

- Load and inspect datasets using Pandas
- Examine data structure, shape, and basic properties
- Identify and analyze missing data patterns
- Calculate descriptive statistics for numerical and categorical data
- Use Pandas methods to gain insights from real-world data
- Document findings and observations clearly

---

## Project Structure

> **Note:** The notebook is fully self-contained — the dataset is loaded directly from a public URL, so no local data files are needed.

---

## Getting Started

### Prerequisites

- Python 3.8+
- Jupyter Notebook or Google Colab
- Pandas, NumPy

### Installation

Clone the repository:

```bash
git clone https://github.com/[your-username]/pandas-eda-tips.git
cd pandas-eda-tips
```

### Part 1: Initial Data Exploration
- Loaded the dataset from a public URL
- Inspected the first and last 5 rows.
- Printed the DataFrame type, shape(244 x 7), and total size (1708 elements)
- Listed all column names and data types
- Examine the default RangeIndex(0-243)
- Checked for missing values across all columns
- Confirmed **zero missing values** anywhere in the dataset

### Part 2: Descriptive Statistics
Numerical columns (total_bill, tip, size):
- Summary statistics via df.describe()
- Mean, median, mode, standard deviation, variance, min/max, and quartiles for total_bill
- Located the highest and lowest bills
- Counted bills above the average

Categorical columns (sex, smoker, day, time):
- Summary via df.dscribe(include=['object])
- Unique values, most frequent value, and frequency per category
- Distribution by day as the closest analog to a regional grouping

### Part 3: Data Quality Assessment
- Checked for duplicate rows (1 found)
- Verified no negative or zero amounts
- Applied the IQR method to detect outliers
- Confirmed consistent categorical formatting across all text columns

### Part 4: Summary and Insight
- Comprehensive dataset overview
- Key findings and patterns
- Data quality report with recommendations

---

### Author
Julia Lee
Course: DSCI 2001-51 Data Science I
Fall Semester 2026 @ North Hennepin Community College
GitHub: @julia-lee



