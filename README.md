# Data-Cleaning-with-SQL
Cleaned the world layoffs data from different companies around the world  with SQL 
Thanks! Now that you've uploaded the **SQL file (`data_cleaning_db.sql`)**, I’ll generate a professional `README.md` using your enhanced GitHub-style template — but tailored to this **SQL Data Cleaning project**.

---

# 🧹 Layoffs Data Cleaning Project

## 📂 About The Project

![Layoffs Data Screenshot](#)

This project is a structured SQL-based data cleaning pipeline applied to a real-world dataset tracking global layoffs across companies, industries, and time. While many datasets are noisy or inconsistent, this project focuses on transforming that raw data into a clean, analysis-ready table using repeatable and transparent SQL techniques.

> Why this project?

* It's easy to skip cleaning, but doing it well is what separates good analysts from great ones.
* This project applies DRY principles by scripting reusable cleaning steps.
* It can be adapted to any messy tabular dataset with minor changes.

The final cleaned dataset can now power dashboards, machine learning models, or reliable reporting.

[(back to top)](#)

---

## 🔧 Built With

This project was developed using:

* **MySQL 8.0+**
* **SQL** — Window functions, CTEs, joins, and updates
* **InnoDB Engine**
* **Structured Pipeline Logic** for reproducibility

[(back to top)](#)

---

## 🚀 Getting Started

To run this project locally, you’ll need to:

### 📦 Prerequisites

* MySQL Server or compatible SQL engine
* SQL client like MySQL Workbench, DBeaver, or DataGrip


## 📈 Usage

The SQL script performs the following cleaning operations:

### ✅ Cleaning Tasks Covered

1. **Remove Duplicates** using `ROW_NUMBER()` and staging tables
2. **Standardize Strings** (e.g., trimming spaces, correcting inconsistent values like `CryptoX`)
3. **Handle Missing Values** by:

   * Replacing blanks with `NULL`
   * Forward-filling missing industries using self-joins
4. **Format Dates** using `STR_TO_DATE()` and altering the column type
5. **Drop Redundant Columns** like `row_num` after use
6. **Schema Control** via `CREATE TABLE` and consistent types

### 🔍 Example:

```sql
UPDATE layoffs_staging2
SET industry = 'Crypto'
WHERE industry LIKE 'Crypto%';
```

[(back to top)](#)

---



## 🙏 Acknowledgments

* [SQL Tutorial – Mode Analytics](https://mode.com/sql-tutorial/)
* [Leetcode SQL Practice](https://leetcode.com/problemset/database/)
* [GitHub Emoji Cheat Sheet](https://www.webpagefx.com/tools/emoji-cheat-sheet/)
* [MySQL Docs](https://dev.mysql.com/doc/)
* [contrib.rocks](https://contrib.rocks)

---

