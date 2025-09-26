# Churn Analysis Project

This project demonstrates an end-to-end **Churn Analysis Pipeline** using **SQL Server, Power BI, and Python**.  
It covers ETL, data cleaning, visualization, and machine learning with Random Forest, integrating results back into Power BI.

---

## 📂 Project Files

- **504c5dce-0774-4f25-8d79-aa8dc07a7ff3.sql**  
  Raw SQL script (uploaded file) containing ETL and data preparation steps for churn dataset.

- **churn_etl.sql**  
  SQL Server script to create schema, clean data, and prepare ML-ready tables.

- **churn_model.ipynb**  
  Jupyter Notebook that builds a Random Forest model, evaluates it, and generates `predicted_churn.csv` for visualization.

- **powerbi_transformations.m**  
  Power Query (M) transformations & DAX measures for Power BI dashboards.

- **README.md**  
  Documentation for setup and usage of the project.

---

## 🚀 Workflow

1. **SQL Server ETL & Cleaning**
   - Run `churn_etl.sql` (or the uploaded `.sql` file) in SQL Server Management Studio.  
   - This will load raw churn data, clean it, and prepare a machine-learning-ready table.

2. **Export Data for ML**
   - Export the cleaned `fact.customers_ml` table to CSV (e.g., `customers_ml.csv`).

3. **Machine Learning in Python**
   - Open `churn_model.ipynb` in Jupyter Notebook.  
   - Load the exported `customers_ml.csv`.  
   - Train a Random Forest model.  
   - Save predictions to `predicted_churn.csv`.

4. **Power BI Integration**
   - Open Power BI Desktop.  
   - Import `customers_ml.csv` and `predicted_churn.csv`.  
   - Use `powerbi_transformations.m` (Power Query & DAX) for transformations and calculated measures.  
   - Create dashboards showing churn KPIs and churner profiles.

---

## 📊 Visuals to Create in Power BI

- **Summary Page**
  - Churn Rate, Customer Demographics, Tenure Distribution, Service Usage.

- **Prediction Page**
  - Churn probability distribution.  
  - Predicted churner profile (age, tenure, service plan).  
  - KPIs for at-risk customers.

---

## 🛠️ Tech Stack

- **SQL Server** – Data ETL & Cleaning  
- **Python (Scikit-learn, Pandas, Numpy)** – Machine Learning  
- **Power BI** – Data Visualization & Dashboarding

---

## 📌 Next Steps

- Replace sample data with real dataset (if available).  
- Fine-tune ML model (e.g., hyperparameter tuning).  
- Add additional Power BI pages for deeper insights.  

---

## 👨‍💻 Author

Aditya Sharma  
B.Tech CSE | Data Analytics Enthusiast | Aspiring Data Analyst  
