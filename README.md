# 🎓 Student Performance Factors Analysis

## 📌 Project Overview
This project analyzes factors that influence student academic performance using SQL (PostgreSQL). The goal was to identify key variables affecting exam outcomes and uncover actionable insights from the dataset.

The analysis was conducted using PostgreSQL in DataCamp DataLab and version-controlled using Git.

---

## 🗂 Dataset Description
The dataset contains student-level information, including:

- Study hours
- Attendance
- Parental education level
- Sleep duration
- Previous exam scores
- Internet access
- Final exam results

File used:
- `StudentPerformanceFactors.csv`

---

## 🛠 Tools & Technologies
- PostgreSQL
- SQL (Joins, Aggregations, Group By, Window Functions)
- DataCamp DataLab
- Git & GitHub
- Jupyter Notebook

---

## 🔎 Key Questions Explored

1. Does study time significantly impact final scores?
2. How does attendance correlate with exam performance?
3. Do students with internet access perform better?
4. What is the relationship between sleep duration and grades?
5. Which factor has the strongest impact on academic success?

---

## 📊 Key Insights

- Students with higher study hours consistently scored above average.
- Attendance showed a strong positive correlation with exam performance.
- Previous exam scores were strong predictors of final results.
- Moderate sleep duration (6–8 hours) was associated with better performance.
- Access to internet resources slightly improved academic outcomes.

---

## 📈 Example SQL Query

```sql
SELECT 
    study_hours, 
    AVG(final_score) AS avg_score
FROM student_performance
GROUP BY study_hours
ORDER BY avg_score DESC;

