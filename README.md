# 📊 Data Science Capstone Project: Manufacturing Equipment Output Prediction  

## 📌 Project Overview  
This project aims to optimize **manufacturing efficiency** by predicting the **hourly output (Parts per Hour)** of injection molding machines based on operational parameters. By building a **Linear Regression model**, the company can:  
- Optimize machine settings.  
- Improve production efficiency.  
- Plan production schedules.  
- Detect underperforming machines.  

---

## 🏷️ Project Details  

**Category:** Supervised Learning (Regression)  
**Problem Statement:** Predict machine output (Parts per Hour) using features such as **temperature, pressure, cycle time, material properties, and machine conditions**.  
**Objective:**  
- Build and evaluate a linear regression model.  
- Provide actionable insights for the production team.  
- Deploy the solution as a **Streamlit web application** hosted on **Streamlit Cloud**.  

---

## 📂 Dataset Information  

**Dataset Name:** `manufacturing_dataset_1000_samples`  
**Size:** 1000 records  
**Target Variable:** `Parts_Per_Hour`  
**Features (17 total):**  
- Injection Temperature  
- Injection Pressure  
- Cycle Time  
- Cooling Time  
- Material Viscosity  
- Ambient Temperature  
- Machine Age  
- Operator Experience  
- Maintenance Hours  
- Shift (Day/Night/Evening)  
- Machine Type (Type_A, Type_B)  
- Material Grade (Economy, Standard, Premium)  
- Day_of_Week (Monday–Sunday)  
- Temperature_Pressure_Ratio  
- Total_Cycle_Time  
- Efficiency Score  
- Machine Utilization  

---

## ⚙️ Data Preprocessing  

1. **Remove/Process Unnecessary Columns**  
   - Drop timestamp or extract useful features (hour/day).  

2. **Handle Missing Values**  
   - `Material_Viscosity`, `Ambient_Temperature`, `Operator_Experience` → Fill with mean/median (numerical) or mode (categorical).  

3. **Encode Categorical Variables**  
   - `Shift`, `Machine_Type`, `Material_Grade`, `Day_of_Week` → One-Hot or Label Encoding.  

4. **Feature Scaling**  
   - Apply `StandardScaler` or `MinMaxScaler` to numerical features for linear regression.  

5. **Define Target Variable**  
   - Target: `Parts_Per_Hour`.  
   - Features: All others after preprocessing.  

---

## 📊 Model Development  

- **Algorithm:** Linear Regression  
- **Dataset Split:** 80% Training | 20% Testing  
- **Evaluation Metrics:**  
  - RMSE, MSE (Regression error metrics)  
  - Precision, Recall, F1-score (if thresholds applied on regression output)  
  - Accuracy (secondary metric)  

---

## 🛠️ Tools & Technologies  

- **Programming:** Python  
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, SciPy, Streamlit  
- **Deployment:** Streamlit Cloud  

---

## 📈 Evaluation  

- **Primary Metrics:** RMSE, MSE, Recall, Precision, F1-score  
- **Secondary Metric:** Accuracy  
- **Deliverables:**  
  - Model Evaluation Report  
  - EDA and Feature Analysis Insights  
  - Final Presentation (15–20 slides)  

---

## 📅 Project Timeline  

| Day | Tasks |
|-----|-------|
| **Day 1** | Data exploration, EDA, preprocessing |
| **Day 2** | Baseline model development & evaluation |
| **Day 3** | Model tuning, evaluation, Streamlit app development |
| **Day 4** | Deployment on Streamlit Cloud, final report & presentation preparation |

---

## 📦 Deliverables  

- **Code Files:** Jupyter notebooks & Python scripts (EDA, model training, evaluation).  
- **Streamlit App:** Interactive web application deployed on **Streamlit Cloud**.  
- **Documentation:** Detailed project report (PDF/Markdown).  
- **Presentation:** 15–20 slide deck summarizing methodology, results, and recommendations.  

---

## 🚀 How to Run the Project  

1. **Clone the Repository**  
   ```bash
   git clone https://github.com/yourusername/manufacturing-output-prediction.git
   cd manufacturing-output-prediction
