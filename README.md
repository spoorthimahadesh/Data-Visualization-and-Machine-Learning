# Data-Visualization-and-Machine-Learning
# 📊 Data Visualization & Machine Learning — Student Performance

A Python-based Jupyter Notebook project that explores student performance data through **data analysis**, **visualizations** (Matplotlib & Seaborn), and a **Logistic Regression ML model** to predict pass/fail outcomes.

---

## 📁 Project Structure

```
📦 part4-visualization-ml
 ┣ 📓 part4_visualization_ml.ipynb
 ┗ 📄 students.csv
```

---

## 📌 Features

### ✅ Task 1 — Exploratory Data Analysis (EDA) with Pandas

- Loads `students.csv` using **Pandas**
- Displays first 5 rows, dataset shape, and column data types
- Generates **summary statistics** (mean, std, min, max, percentiles)
- Counts passed vs failed students
- Calculates **average subject scores** separately for passed and failed students
- Identifies the **top student** with the highest overall average

### ✅ Task 2 — Data Visualization with Matplotlib

5 charts generated and saved as `.png` files:

| Plot | Type | Description |
|------|------|-------------|
| Plot 1 | Bar Chart | Average score per subject |
| Plot 2 | Histogram | Distribution of Math scores with mean line |
| Plot 3 | Scatter Plot | Study hours per day vs average score (Pass/Fail color-coded) |
| Plot 4 | Box Plot | Attendance distribution — Pass vs Fail |
| Plot 5 | Line Plot | Math and Science scores per student |

### ✅ Task 3 — Advanced Visualization with Seaborn

- **Grouped Bar Plot** — Average Math & Science score by Pass/Fail
- **Scatter Plot with Regression Line** — Attendance % vs Average Score (Pass/Fail trend lines)
- Includes a written comparison of **Seaborn vs Matplotlib**

### ✅ Task 4 — Machine Learning with Scikit-learn

A complete ML pipeline to predict whether a student will pass or fail:

| Step | Description |
|------|-------------|
| 1 | Feature/target split — 7 features, `passed` as target |
| 2 | Train/test split — 80% train, 20% test (`random_state=42`) |
| 3 | Feature scaling using **StandardScaler** |
| 4 | Model training using **Logistic Regression** (`max_iter=500`) |
| 5 | Accuracy evaluation on both train and test sets |
| 6 | Feature importance via model **coefficients** (horizontal bar chart) |
| 7 | Prediction on a **new student's data** |

---

## 📂 Dataset — `students.csv`

| Column | Type | Description |
|--------|------|-------------|
| `name` | string | Student name |
| `math` | int | Math score |
| `science` | int | Science score |
| `english` | int | English score |
| `history` | int | History score |
| `pe` | int | Physical Education score |
| `attendance_pct` | int | Attendance percentage |
| `study_hours_per_day` | float | Daily study hours |
| `passed` | int | 1 = Pass, 0 = Fail |

> Dataset contains **15 students** — 9 passed, 6 failed.

---

## 🚀 Getting Started

### Prerequisites

- Python 3.x
- Jupyter Notebook or JupyterLab

### Install Dependencies

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

### Run the Notebook

```bash
# Clone the repository
git clone https://github.com/your-username/part4-visualization-ml.git

# Navigate into the folder
cd part4-visualization-ml

# Launch the notebook
jupyter notebook part4_visualization_ml.ipynb
```

> Make sure `students.csv` is in the **same directory** as the notebook before running.

---

## 🛠️ Built With

| Library | Purpose |
|---------|---------|
| **Pandas** | Data loading and analysis |
| **NumPy** | Numerical operations |
| **Matplotlib** | Data visualization |
| **Seaborn** | Advanced statistical visualization |
| **Scikit-learn** | Machine learning pipeline |

---

## 👩‍💻 Author

**Spoorthi M**  
**Student_id : bitsom_ba_2511762**

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
