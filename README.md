# Student Performance EDA (Python) + Power BI Dashboard

## Overview
This project performs **Exploratory Data Analysis (EDA)** on a student performance dataset to understand how demographic and academic-related factors influence **Math, Reading, and Writing** scores. The workflow includes data cleaning, visualization, feature engineering, performance segmentation, and correlation analysis. The final cleaned dataset is prepared for a **single-page Power BI dashboard**.

---

## Objectives
- Explore the distribution of student scores across subjects.
- Analyze the impact of:
  - **Gender**
  - **Race/Ethnicity**
  - **Parental level of education**
  - **Lunch type**
  - **Test preparation course**
- Engineer features for dashboard-ready insights:
  - **Total Score**
  - **Performance Level (Low/Medium/High)**
- Identify relationships between subject scores using correlation analysis.

---

## Dataset
The dataset contains student-level records with the following key columns:
- **Demographics:** `gender`, `race/ethnicity`, `parental_level_of_education`
- **Support factors:** `lunch`, `test_preparation_course`
- **Scores:** `math_score`, `reading_score`, `writing_score`

**Feature Engineering added:**
- `total_score` = math + reading + writing
- `performance_level` = Low / Medium / High (based on total score thresholds used in the notebook)

---

## Tools & Technologies
- **Python**
- **Pandas** (data wrangling)
- **Matplotlib & Seaborn** (visualizations)
- **Jupyter Notebook** (analysis)
- **Power BI** (single-page dashboard design)

---

## Project Workflow
1. **Data Loading & Inspection**
   - Checked dataset shape, column types, unique categorical values
   - Verified missing values and overall consistency

2. **Data Cleaning**
   - Standardized column names (spaces → underscores for easier use)
   - Ensured numeric columns are correctly treated as scores

3. **Exploratory Visualizations**
   - Score distributions across subjects
   - Category-wise comparisons (gender, lunch, test prep, parental education, race/ethnicity)

4. **Key Analytical Questions Covered**
   - **Parental education vs Math performance**
   - **Gender-wise performance differences**
   - **Effect of test preparation course**
   - **Top performers (top 10%) segmentation**
   - **Lunch impact across different race/ethnicity groups**

5. **Correlation Analysis**
   - Computed relationships among `math_score`, `reading_score`, `writing_score`
   - Observed strong correlation between **reading and writing**, and comparatively lower correlation between **math and writing**

6. **Feature Engineering for Dashboard**
   - Created `total_score` and `performance_level`
   - Exported a cleaned dataset suitable for Power BI reporting

---

## Key Insights (Summary)
- **Test preparation** is associated with higher average scores across subjects.
- **Lunch type** shows a clear performance gap: students with **standard lunch** generally score higher than **free/reduced**.
- **Gender trend**: males tend to score higher in **math**, while females tend to score higher in **reading/writing**.
- **Parental education** generally shows a positive relationship with student performance.
- **Reading and writing** scores move closely together (very strong correlation).

---

## Power BI Dashboard (Single Page)
The dashboard is designed to be a clean, one-page view including:
- KPI Cards (Avg Math/Reading/Writing + Student Count)
- Score comparisons by key factors (gender, parental education, lunch, test prep)
- Performance Level distribution (Low/Medium/High)
- Interactive slicers for quick filtering

---

## Repository Structure (Suggested)
- `EDA_Student_Performance_Analysis.ipynb` → EDA Notebook
- `final_student_performance.csv` → Dataset / cleaned output (if included)
- `README.md` → Project documentation
- `Dashboard/` → Power BI files or screenshots (optional)

---

## Links

- GitHub Repo: 
- LinkedIn: https://www.linkedin.com/in/ghulam-murtaza-b24280331?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=android_app
