# 🇧🇷 Brazilian Universities Data ETL

This project demonstrates a simple **ETL (Extract, Transform, Load)** process that collects, processes, and stores data about Brazilian universities using Python, Pandas, and SQLite.

---

## 🧩 Process Overview

### 1. **Extract**
Data is fetched from the **[Universities Hipolabs API](https://universities.hipolabs.com/)**, which provides public information about universities worldwide.

### 2. **Transform**
The raw data is:
- Converted into a **Pandas DataFrame**.  
- **Filtered** to include only universities located in the state of **Goiás**.  
- **Formatted** to include selected columns such as name, country, domain, and web page.

### 3. **Load**
The cleaned and transformed data is:
- Saved locally as a **CSV file** (`universities.csv`).  
- Inserted into an **SQLite database** (`my_lite_store.db`) under the table **`goias_uni`**.

---

## 📁 Project Files

| File | Description |
|------|--------------|
| `Brazilian_Universities_ETL.ipynb` | The Jupyter Notebook containing the full ETL code. |
| `my_lite_store.db` | SQLite database containing the processed data. |
| `universities.csv` | CSV file containing the transformed dataset prior to loading into the database. |

---

## ⚙️ How to Run

1. **Open** the notebook in [Google Colab](https://colab.research.google.com) or a local **Jupyter environment**.  
2. **Run all cells sequentially** to perform the ETL process.  
3. After execution, the files `my_lite_store.db` and `universities.csv` will be generated in the same directory as the notebook.

---

## 🧰 Requirements

- Python 3.8+
- pandas
- requests
- sqlite3 (included in Python standard library)

Install dependencies:
```bash
pip install pandas requests
