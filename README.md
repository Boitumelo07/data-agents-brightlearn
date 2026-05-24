# Retail Sales Data Agent on Databricks

## Project Overview
This project is a working Data Agent built on Databricks that answers business questions about retail sales data. The agent allows non-technical users like business owners and store managers to ask questions in plain English and receive accurate, data-driven insights.

## Dataset
The retail sales dataset contains **1,000 transactions** with the following columns:

| Column | Type | Description |
|--------|------|-------------|
| Transaction ID | bigint | Unique identifier for each sale |
| Date | date | Transaction date |
| Customer ID | string | Anonymous customer identifier |
| Gender | string | Customer gender (Male/Female) |
| Age | bigint | Customer age (18-64 years) |
| Product Category | string | Electronics / Clothing / Beauty |
| Quantity | bigint | Number of units purchased |
| Price per Unit | bigint | Cost per single unit |

## Tools Used
- **Databricks** – Genie Spaces, SQL Editor, Catalog Explorer
- **GitHub** – Version control and submission

## Agent Instructions Summary
The agent was given custom instructions to:
- Use only the retail_sales_data dataset
- Answer questions about sales, customers, products, and trends
- Never invent numbers or make assumptions
- Provide clear, professional, business-focused insights
- Ask for clarification when questions are unclear

## 10 Test Questions and Answers

| # | Question | Answer |
|---|----------|--------|
| 1 | What is total revenue? | $456,000 |
| 2 | Which product category has the highest sales? | Electronics ($156,905) |
| 3 | What is the average age of customers? | 41.4 years |
| 4 | Show sales by gender | Female $232,840 / Male $223,160 |
| 5 | What are monthly sales trends? | Peak May $53,150 / Low Sep $23,620 |
| 6 | Which product category has the highest quantity sold? | Clothing (894 units) |
| 7 | What is the average transaction value? | $456 |
| 8 | Which age group spends the most? | 45-54 ($97,235) |
| 9 | Compare sales between Electronics and Beauty | Electronics leads by $13,390 |
| 10 | Best category for customers under 30? | Clothing ($46,150) |

## Validation of Answers
Three answers were validated using SQL queries against the raw dataset:

| Validation | Agent Answer | SQL Result | Verdict |
|------------|--------------|------------|---------|
| Total Revenue | $456,000 | 456,000 | ✅ Correct |
| Average Age | 41.4 years | 41.392 | ✅ Correct |
| Sales by Gender (Female) | $232,840 | 232,840 | ✅ Correct |
| Sales by Gender (Male) | $223,160 | 223,160 | ✅ Correct |

## Key Business Insights
- **Electronics** generates the highest revenue ($156,905) but sells fewer units (849) – higher priced items
- **Clothing** sells the most units (894) but revenue is slightly lower – volume driver
- **Female customers** spend $9,680 more than male customers
- **Age group 45-54** spends the most ($97,235)
- **Sales peak in May** ($53,150) and dip in September ($23,620)

## Business Recommendations
1. **Increase Electronics inventory before May** – Highest revenue category peaks in May
2. **Target age 45-54 with loyalty programs** – They spend the most money
3. **Bundle Clothing with Electronics** – Clothing drives volume, Electronics drives value
4. **Investigate September sales dip** – Consider back-to-school promotion

## Repository Contents
- `Building_a_Retail_Sales_Data_Agent.docx` – Full project write-up
- `/screenshots` – All screenshots from each step
- `README.md` – This file

## Author
Boitumelo Zwane
2805001656

24 May 2026

## Course
BrightLearn – Data Agent Task
