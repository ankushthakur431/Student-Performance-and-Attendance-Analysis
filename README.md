# 📊 Student Performance and Attendance Analysis

## 📌 Project Overview

This project analyzes student academic performance and attendance using Python libraries such as **Pandas**, **NumPy**, and **Matplotlib/Seaborn**.

The dataset consists of two Excel sheets:

* **Student Marks**
* **Student Attendance**

The main objective is to combine, clean, and analyze the data to generate meaningful insights for decision-making.

---

## 🎯 Objectives

* Calculate total marks and percentage for each student
* Derive attendance percentages
* Compute weighted performance scores
* Classify students based on performance levels
* Identify low attendance students and top performers
* Visualize trends and patterns in the dataset

---

## 🛠️ Technologies Used

* Python 🐍
* Pandas
* NumPy
* Matplotlib
* Seaborn
* OpenPyXL (for Excel handling)

---

## 📂 Dataset Description

The Excel file contains two sheets:

1. **Marks Sheet**

   * Name
   * Mini Test 1
   * Mini Test 2
   * Live Test
   * Assignment

2. **Attendance Sheet**

   * Name
   * Multiple attendance columns (Y/N format)

---

## 🔄 Data Preparation Steps

1. Load Excel file into two DataFrames
2. Merge DataFrames using the **Name** column
3. Convert attendance values:

   * `Y → 1`
   * `N → 0`
4. Handle missing values
5. Clean column formats (standardize names)

---

## 🔢 Data Transformation

New columns created:

* **Total Marks**
* **Percentage Marks**
* **Attendance Percentage**
* **Weighted Percentage**

### 📐 Weighted Formula:

```
Weighted Score = 
(Attendance × 40%) + 
(Mini Test 1 × 10%) + 
(Mini Test 2 × 10%) + 
(Live Test × 20%) + 
(Assignment × 20%)
```

---

## 🏆 Performance Classification

| Percentage Range | Category          |
| ---------------- | ----------------- |
| ≥ 85             | Excellent         |
| 71 – 84          | Good              |
| 50 – 70          | Average           |
| < 50             | Needs Improvement |

---

## 📊 Analysis Performed

* Identified students with:

  * Attendance < 75%
  * Weighted Percentage > 50%
* Extracted **Top 3 performers**
* Studied **impact of attendance on performance**

---

## 📈 Visualizations

The following charts were created:

1. 📊 **Bar Chart**

   * Top 5 students based on weighted percentage

2. 🥧 **Pie Chart**

   * Distribution of performance categories

3. 📦 **Box Plots**

   * Mini Test 1
   * Mini Test 2
   * Live Test
   * Assignment

4. ⚠️ **Low Attendance Chart**

   * Students with attendance < 50%

5. 📉 Additional Insights

   * Relationship between attendance and marks

---

## 🚀 How to Run the Project

1. Clone the repository:

```
git clone https://github.com/your-username/student-performance-analysis.git
```

2. Install required libraries:

```
pip install pandas numpy matplotlib seaborn openpyxl
```

3. Run the Python script:

```
python main.py
```

---

## 📌 Key Insights

* Higher attendance generally leads to better performance
* Some students perform well despite low attendance
* Outliers detected in test scores
* Clear segmentation of students based on performance

---

## 📎 Future Improvements

* Add machine learning model for performance prediction
* Build dashboard using Streamlit or Power BI
* Automate report generation

---

## 👤 Author

**Ankush Thakur**
Mechanical Engineer | Python & Data Analysis Enthusiast

---

## ⭐ If you like this project

Give it a star ⭐ on GitHub!

