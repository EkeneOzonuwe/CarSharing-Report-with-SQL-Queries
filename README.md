# 🚗 CarSharing Report with SQL Queries

A end-to-end data analysis project using a real car-sharing dataset (Jan 2017 – Aug 2018). The project covers data cleaning in Google Sheets, relational database design in SQLite, and SQL-based business reporting.

---

## 📋 Project Brief

Analysed hourly car-sharing demand data to answer key business questions for a fictional manager, Linda. The dataset included customer demand rates alongside time, weather, and temperature data.

---

## 🗄️ Database Design

The raw data was cleaned and split into four relational tables:

| Table | Key Columns |
|-------|-------------|
| `CarSharing_df` | id, demand, weather_code, temp_code |
| `time` | id, timestamp, season, hour, weekday, month |
| `temperature` | temp_code, temp, temp_feel, temp_category |
| `weather` | weather_code, weather condition |

Tables are linked via foreign keys to form a star schema (see ERD).

---

## 📊 Business Questions Answered

**(a) Highest Demand in 2017**
Identified the exact date and hour with peak customer demand.

**(b) Highest & Lowest Average Demand**
Compared weekday, month, and season to find when demand was strongest and weakest throughout 2017.

**(c) Hourly Demand Breakdown**
For the highest/lowest demand weekdays, produced an hourly average demand table sorted in descending order.

**(d) Weather Analysis — 2017**
- Most prevalent temperature category (Cold / Mild / Hot)
- Most common weather condition
- Average, highest, and lowest wind speed per month
- Average, highest, and lowest humidity per month
- Average demand by temperature category

**(e) Best Month Deep-Dive**
Repeated the weather analysis for the highest-demand month to enable direct comparison.

---

## 🛠️ Tools Used

- **Google Sheets** — data cleaning, missing value imputation, feature engineering
- **SQLite** — database creation, table imports, relational linking
- **SQL** — all business queries (aggregations, joins, grouping, sorting)
- **GitHub** — documentation and collaboration

---

## 💡 SQL Skills Demonstrated

`JOIN` · `GROUP BY` · `ORDER BY` · `AVG / MIN / MAX` · `WHERE` · `HAVING` · Subqueries · Date filtering · Multi-table relational queries

---

## 📁 Files

- `CarSharing_df.csv` — main dataset
- SQL query file — all queries with comments per question

---

*Project completed as part of a data analytics course. Dataset covers Jan 2017 – Aug 2018.*
