# 🧹 Data Cleaning Pipeline (Stocks & Energy Data)

A lightweight Python project demonstrating **data preprocessing and cleaning techniques** on structured datasets (stocks & energy consumption).

This project focuses on transforming raw, inconsistent data into **clean, validated, and analysis-ready datasets** — a core step in any **data engineering / ML pipeline**.

---

## 📌 Overview

The script processes two datasets:

### 📊 Stock Market Data
- Fields: `Date`, `Stock`, `Open`, `Close`, `Volume`

### ⚡ Energy Consumption Data
- Fields: `Date`, `Energy_Type`, `Consumption`, `Price`

---

## 🎯 Objectives

- Handle **missing values**
- Convert **data types (string → datetime, float, int)**
- Normalize **categorical fields**
- Remove **invalid records**
- Produce **clean datasets ready for downstream tasks**

---

## 🛠️ Data Cleaning Steps

### 1. Date Standardization
- Converts string dates → `datetime` objects
- Invalid formats are handled gracefully

### 2. Missing Value Handling

| Field Type | Strategy |
|------------|--------|
| Numerical  | Replace with `0` / `0.0` |
| Date       | Set to `None` |
| Category   | Default to `"unknown"` |

---

### 3. Type Conversion

- `Open`, `Close` → `float`
- `Volume` → `int`
- `Consumption`, `Price` → `float`

---

### 4. Categorical Cleaning

- Removes whitespace
- Converts to lowercase
- Ensures consistency

---

### 5. Data Validation

Only valid rows are retained:
- Must have a valid `Date`
- Must have required categorical fields

---

## ⚙️ How to Run

```bash
python main.py
```

---

## 📦 Tech Stack

- Python 3.x  
- Standard Library (`datetime`)  

---

## 🚀 Real-World Applications

- 📊 Financial data preprocessing  
- ⚡ Energy analytics pipelines  
- 🤖 ML feature engineering  
- 🧾 ETL pipelines (Extract → Transform → Load)  

---

## ⭐ Support

If you found this useful, consider giving it a ⭐ on GitHub!
