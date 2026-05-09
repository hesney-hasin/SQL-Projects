# 🗄️ SQL Projects 

A collection of guided SQL projects completed on [DataCamp](https://www.datacamp.com/) as part of my journey toward becoming a Data Analyst. Each project uses real-world datasets and explores a distinct domain — from global finance to public transport to mental health research.

---

## 📁 Projects

### 1. 🌍 Analyzing International Debt Statistics
**File:** `workspace/` (World Bank dataset)

**Overview:**
Analyzed international debt data collected by The World Bank to understand how much debt developing countries owe across various categories.

**Key Questions Answered:**
- How many distinct countries are present in the database?
- Which country carries the highest total debt?
- Which country has the lowest principal repayments?

**Concepts Practiced:**
- `SELECT DISTINCT`, `COUNT`
- `SUM` with `GROUP BY`
- `ORDER BY` + `LIMIT` for ranking
- Filtering with `WHERE` using indicator codes

**Dataset Schema — `international_debt`:**

| Column | Description | Type |
|---|---|---|
| `country_name` | Name of the country | `VARCHAR` |
| `country_code` | Country code | `VARCHAR` |
| `indicator_name` | Description of the debt indicator | `VARCHAR` |
| `indicator_code` | Code for the debt indicator | `VARCHAR` |
| `debt` | Debt amount in current USD | `FLOAT` |

---

### 2. 🚇 Exploring London's Travel Network
**File:** `workspace__1_/` (Transport for London dataset)

**Overview:**
Queried a Google BigQuery database of Transport for London (TfL) journey data to understand travel patterns across different transport modes in London.

**Key Questions Answered:**
- Which transport types are most popular overall?
- What were the peak months for the Emirates Airline cable car?
- Which years saw the lowest Underground journey volumes?

**Concepts Practiced:**
- `SUM` with `GROUP BY` and `ORDER BY` for aggregation
- `ROUND` for formatting output
- `LIKE` with wildcard patterns (`%Underground%`)
- Filtering `NULL` values with `IS NOT NULL`
- Multi-column `ORDER BY`

**Dataset Schema — `TFL.JOURNEYS`:**

| Column | Description | Type |
|---|---|---|
| `MONTH` | Month number (1 = January) | `INTEGER` |
| `YEAR` | Year | `INTEGER` |
| `DAYS` | Number of days in the month | `INTEGER` |
| `REPORT_DATE` | Date the data was reported | `DATE` |
| `JOURNEY_TYPE` | Method of transport used | `VARCHAR` |
| `JOURNEYS_MILLIONS` | Journeys in millions | `FLOAT` |

---

### 3. 🧠 Analyzing Students' Mental Health
**File:** `workspace__2_/` (PostgreSQL — university survey dataset)

**Overview:**
Used PostgreSQL to explore a 2018 survey from a Japanese international university, investigating whether international students are at higher risk of mental health difficulties and whether length of stay is a contributing factor.

**Key Questions Answered:**
- Do international students show higher depression, lower social connectedness, or higher acculturative stress?
- How do these scores vary by length of stay?

**Concepts Practiced:**
- Filtering with `WHERE` on categorical values
- `COUNT`, `AVG`, `ROUND` for descriptive statistics
- `GROUP BY` + `ORDER BY` for segmented analysis
- Working with psychological scale scores (PHQ-9, SCS, ASISS)

**Dataset Schema — `students`:**

| Column | Description |
|---|---|
| `inter_dom` | Student type: International or Domestic |
| `japanese_cate` | Japanese language proficiency |
| `english_cate` | English language proficiency |
| `academic` | Academic level (undergraduate/graduate) |
| `age` | Student age |
| `stay` | Length of stay in years |
| `todep` | Depression score (PHQ-9) |
| `tosc` | Social connectedness score (SCS) |
| `toas` | Acculturative stress score (ASISS) |

---

### 4. 📓 Introduction to DataCamp Notebooks
**File:** `workspace__3_/`

**Overview:**
An introductory walkthrough of the DataCamp notebook environment. Covers how SQL cells, text cells, DataFrames, and the submission/testing system work — the foundation for all other projects in this repository.

**Concepts Covered:**
- How notebooks are structured (text cells vs. SQL cells)
- Running SQL against live databases in the DataCamp environment
- Understanding DataFrames and result validation
- Submission workflow and interpreting test feedback

---

## 🛠️ Tools & Technologies

| Tool | Usage |
|---|---|
| **SQL (PostgreSQL / BigQuery)** | Primary query language across all projects |
| **DataCamp Workspace** | Notebook environment for running SQL |
| **Google BigQuery** | Used in the TfL project |
| **PostgreSQL** | Used in the mental health project |

---

## 📚 Skills Demonstrated

- Writing analytical SQL queries from scratch
- Aggregation and grouping (`SUM`, `COUNT`, `AVG`, `GROUP BY`)
- Filtering and sorting (`WHERE`, `ORDER BY`, `LIMIT`)
- String pattern matching (`LIKE`)
- Working with `NULL` values
- Interpreting real-world datasets across multiple domains

---

## 🚀 About

These projects were completed as part of the **DataCamp SQL learning track**. They represent hands-on practice with real datasets across finance, transportation, and social science — moving from SQL fundamentals toward more applied data analysis.

> **Currently learning:** SQL → Python for Data Analysis → Machine Learning  
> **Goal:** Data Analyst → Data Scientist

---

## 📬 Connect

- 🐙 GitHub: [@hesneyhasin](https://github.com/hesneyhasin)
- 💼 Open to internship opportunities in Data Analysis & AI

---

*Projects completed on DataCamp. Datasets sourced from The World Bank, Transport for London (TfL), and academic research.*
