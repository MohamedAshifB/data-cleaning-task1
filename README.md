# data-cleaning-task1
Data Cleaning and Preprocessing task for internship


# 🧹 Task 1 - Data Cleaning and Preprocessing

This project is part of the **Data Analyst Internship**. The goal was to clean and prepare a raw dataset using Python (Pandas).

---

## 📁 Dataset Used

**Medical Appointment No Shows**  
Source: [Kaggle - No-show appointments](https://www.kaggle.com/datasets/joniarroba/noshowappointments)

---

## ✅ Cleaning Steps Performed

1. **Loaded** the raw dataset `KaggleV2-May-2016.csv` using Pandas.
2. **Dropped irrelevant columns**: `PatientId`, `AppointmentID`.
3. **Renamed column headers** to lowercase and removed spaces/hyphens.
4. **Converted date columns** (`scheduled_day`, `appointment_day`) to datetime format.
5. **Standardized categorical fields**:
   - `gender`: converted to uppercase
   - `no_show`: mapped `NO` → `0` (showed up), `YES` → `1` (missed)
6. **Checked and cleaned data types** (ensured `age` is integer and removed invalid ages).
7. **Removed duplicate rows** from the dataset.
8. **Checked for missing values** — no nulls found.
9. **Saved** the cleaned dataset as `cleaned_medical_appointments.csv`.

---

## 🧼 Final Output

A clean, structured dataset ready for analysis or modeling:
- 0 = Patient showed up
- 1 = Patient missed the appointment

---

## 📂 Files in this Repo

- `Task_1_.ipynb` – Jupyter Notebook with code
- `KaggleV2-May-2016.csv` – Original dataset
- `cleaned_medical_appointments.csv` – Final cleaned dataset
- `README.md` – This summary

---

## 🧠 Concepts Practiced

- Handling missing values
- Removing duplicates
- Text standardization
- Date/time conversion
- Column renaming and formatting
- Data type validation

---

## 🚀 How to Run

```bash
# Clone the repo and run the notebook
jupyter notebook Task_1_.ipynb
