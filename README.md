# StudentMarksAnalyse
# 📊 Student Marks Analysis using Python 🧠

This project aims to perform an in-depth exploratory data analysis (EDA) on a student marks dataset using Python. The dataset contains academic scores along with various demographic and socio-economic factors. We use this information to uncover performance patterns and insights that can help improve learning strategies and educational outcomes.

---

## 🧾 Dataset Description

The dataset used in this project is:
**`Expanded_data_with_more_features.csv`**

Each row represents a student record, and the dataset includes the following columns:

| Column Name            | Description |
|------------------------|-------------|
| `Gender`               | Gender of the student (male/female) |
| `EthnicGroup`          | Student's ethnic background |
| `ParentEduc`           | Level of education of the parents |
| `LunchType`            | Type of lunch received (free/reduced/standard) |
| `TestPrep`             | Whether the student completed a test preparation course |
| `ParentMaritalStatus`  | Marital status of the student's parents |
| `PracticeSport`        | Whether the student practices sports |
| `IsFirstChild`         | Whether the student is the first child |
| `NrSiblings`           | Number of siblings |
| `TransportMeans`       | How the student travels to school |
| `WklyStudyHours`       | Weekly study hours spent by the student |
| `MathScore`            | Score in Mathematics (0-100) |
| `ReadingScore`         | Score in Reading (0-100) |
| `WritingScore`         | Score in Writing (0-100) |

---

## 🔍 Objective

- Understand the distribution of students by demographics.
- Examine the relationship between performance and socio-economic factors.
- Identify key factors that affect students' academic performance.
- Classify overall student performance into categories for better insight.

---

## 📈 Analysis Performed

### 1. **Gender Distribution**
- Used a `countplot()` to visualize the number of male and female students.
- **Observation**: More female students than male students.

### 2. **Subject-wise Outlier Detection**
- Plotted boxplots for `MathScore`, `ReadingScore`, and `WritingScore`.
- **Observation**: Found subject-specific variations and outliers.

### 3. **Weekly Study Hours vs Scores**
- Boxplots used to see how `WklyStudyHours` impact scores.
- **Insight**: Slight impact on Math, but less noticeable effect on other subjects.

### 4. **Overall Performance Calculation**
- Calculated average of all 3 subjects for each student.
- Created performance categories using `pd.cut()`:
  - 0–50 → Poor
  - 51–70 → Average
  - 71–90 → Good
  - 91–100 → Excellent

### 5. **Gender-wise Performance**
- Barplots to compare average scores across genders.
- **Insight**: Males slightly outperform females in Reading & Writing.

### 6. **Parent Education vs Marks**
- Grouped by `ParentEduc` and plotted a heatmap of mean scores.
- **Insight**: Higher parent education level correlates with better student scores.

### 7. **Parent Marital Status vs Marks**
- Grouped by `ParentMaritalStatus` and visualized.
- **Insight**: No significant effect observed.

### 8. **Test Preparation vs Scores**
- Grouped by `TestPrep` and visualized via heatmap.
- **Insight**: Test prep has a clear positive impact on scores.

---

## 🧠 Key Insights & Conclusions

1. **Test Preparation Helps** – Students who completed test prep scored significantly higher in all subjects.
2. **Parental Education is Key** – Children of highly educated parents tend to perform better.
3. **Gender Impact Exists** – Gender-wise performance differences observed, especially in Reading and Writing.
4. **Weekly Study Time Matters Slightly** – Especially visible in Math performance.
5. **Parent Marital Status has Limited Effect** – Does not notably affect student scores.

---

## 📦 Technologies Used

- Python 3.x
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Google Colab (for notebook-based analysis)

---

## 📁 Project Structure

```bash
studentmarksanalyse.py       # Main analysis script
README.md                    # Project overview and findings
Expanded_data_with_more_features.csv  # Dataset used
