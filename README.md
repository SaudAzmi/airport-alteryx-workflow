# ✈️ Airport – City Population Enrichment (Alteryx Workflow)

## 📌 Project Overview
This project demonstrates an end-to-end data preparation workflow built in **Alteryx** to enrich airport data with demographic information from global city datasets.

The goal was to combine two independent data sources and produce a clean, validated dataset where each airport is matched with its corresponding city and population.

The workflow focuses not only on joining datasets, but also on **data quality validation, duplicate handling, and reliable matching logic** — reflecting real-world analytics practices.

---

## 🎯 Objective
Create a reproducible workflow that:

- Integrates airport and city datasets
- Ensures accurate city matching
- Handles duplicate and inconsistent records
- Produces a structured analytical output file

---

## 🧠 Workflow Design Philosophy
Rather than performing a direct join, the workflow follows a structured data engineering approach:

1. **Understand the data**
2. **Validate quality**
3. **Standardize inputs**
4. **Control matching logic**
5. **Produce business-ready output**

---

## ⚙️ Workflow Stages

### 🔎 Data Profiling
- Reviewed dataset structure and field types
- Checked null values and completeness
- Identified potential join risks

### 🧩 Duplicate Detection
- Detected duplicate city-country combinations
- Prevented one-to-many joins
- Aggregated records for controlled matching

### 🧹 Data Cleansing
- Removed whitespace and hidden characters
- Cleaned join fields to improve reliability

### 🔤 Data Standardization
- Created standardized join keys:
  - `City_clean`
  - `Country_clean`
- Applied consistent casing and formatting

### 🔗 Join Logic
- Joined datasets using **City + Country**
- Avoided incorrect matches between cities sharing names
- Validated matched and unmatched outputs

### 📊 Output Preparation
- Selected analytical fields
- Improved column readability
- Structured dataset for reporting use

---

## 🛠 Tools Used
- Input Data
- Browse
- Field Summary
- Data Cleansing
- Formula
- Summarize
- Filter
- Join
- Select
- Output Data

