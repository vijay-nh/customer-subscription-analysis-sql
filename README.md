# Customer Subscription Analysis - SQL Project 4

## 📌 Project Overview
This project analyses customer subscription data for a SaaS company 
using MySQL. It covers revenue analysis, customer segmentation, 
churn risk identification, support ticket analysis and plan 
performance — across 3 related tables using JOINs and Subqueries.

---

## 🛠️ Tools Used
- MySQL
- MySQL Workbench

---

## 📊 Dataset
Three related tables — Customers, Subscriptions and Support Tickets

### Customers Table
| Column | Description |
|---|---|
| customer_id | Unique identifier |
| customer_name | Name of the customer |
| customer_city | City of the customer |
| industry | Industry sector |
| signup_date | Date they signed up |

### Subscriptions Table
| Column | Description |
|---|---|
| subscription_id | Unique identifier |
| customer_id | Links to customers table |
| plan_type | Starter / Professional / Enterprise |
| monthly_fee | Fee paid per month |
| start_date | Subscription start date |
| end_date | Subscription end date |
| status | Active or Cancelled |

### Support Tickets Table
| Column | Description |
|---|---|
| ticket_id | Unique identifier |
| customer_id | Links to customers table |
| issue_type | Type of issue raised |
| raised_date | Date ticket was raised |
| resolved | Whether ticket was resolved |

---

## 🔍 Key Business Questions Answered

1. Which plan type generates the most monthly revenue?
2. Which industry has the most active customers?
3. Which customers pay above the average monthly fee?
4. Which customers pay the highest monthly fee?
5. How does each customer's fee compare to the overall average?
6. Which industries have more than 1 active customer?
7. Which customers have raised support tickets?
8. Which cancelled customers had unresolved tickets?
9. Who are the highest ticket raisers and are they still active?
10. Which customers are potential churn risks?

---

## 💡 Key Insights

- **Enterprise** plan generates the highest total monthly revenue
- **HRMS and IT** industries have the most active customers
- Cancelled customers consistently had **more unresolved tickets**
- Customers with **3+ support tickets** show highest churn risk
- **Corporate segment** customers contribute more revenue on average

---

## 🧠 New SQL Concepts Practised

- Subquery in WHERE clause
- Subquery in SELECT clause  
- Subquery in FROM clause
- HAVING clause — filtering after GROUP BY
- 3 table JOINs
- MAX() and AVG() aggregate functions
- Churn risk analysis using ticket data
- Customer segmentation using CASE + JOIN

---

## 🚀 What I Learned
- How to write queries inside queries (subqueries)
- How to filter grouped results using HAVING
- How to join 3 tables simultaneously
- How to identify churn risk patterns using support data
- How to compare individual values against overall averages
- Real SaaS business analysis patterns used by analysts daily
