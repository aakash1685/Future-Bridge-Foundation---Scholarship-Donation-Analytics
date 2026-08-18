# Future Bridge Foundation — Scholarship & Donation Analytics

### Turning donations into opportunities.

Every scholarship has a story behind it.

A donor contributes to a foundation.
The foundation receives and manages those funds.
Those funds are then directed toward students pursuing their education.

But when the number of donors, students, universities, institutes, cities, and transactions grows, answering simple questions becomes difficult:

- Where is the money coming from?
- Who are the major contributors?
- Which cities and donor categories contribute the most?
- Which universities and institutes receive the most scholarship support?
- How many students are being supported?
- What is the academic and financial profile of supported students?
- How are scholarship funds being distributed?

**This Power BI project was built to turn those questions into meaningful insights.**

---

## About the Project

Future Bridge Foundation is a fictional education-focused foundation used as the business scenario for this analytics project.

The project simulates a foundation operating across Gujarat, receiving donations from individuals, corporations, and family foundations and distributing scholarships to college students.

The objective is not simply to create charts, but to understand the complete flow of financial and educational support:

**Donors → Donations → Scholarship Distribution → Students**

The dashboard analyzes foundation data for the period:

**01 April 2024 – 31 May 2025**

---

## The Data Story

The project connects multiple aspects of the foundation's operations.

### Donor Side

The foundation receives contributions from:

- Individual Donors
- Corporate Donors
- Family Foundations

### Scholarship Side

Scholarship funds are distributed across:

- Universities
- Institutes
- Courses
- Public and Private Institutions

### Student Side

Students are analyzed based on:

- City
- Course
- Academic Performance
- Family Annual Income
- Gender
- University
- Institute

This structure allows the dashboard to move from a foundation-level overview to detailed donor, scholarship, and student analysis.

---

# Dashboard Pages

## 01 — Foundation Overview

The Foundation Overview provides a high-level picture of the foundation's operations.

### Key KPIs

- Total Donors — 250
- Total Universities — 10
- Total Institutes — 15
- Students Supported — 2.00K
- Total Donations — ₹796.81M
- Distributed Scholarship — ₹76.96M

### Key Analysis

- Donor Contribution by Category
- Scholarship Distribution by University
- Top 5 Donors by Contribution
- Students Supported by Course

This page provides the starting point for understanding the foundation's overall financial and educational impact.

---

## 02 — Donor Analysis

The Donor Analysis page focuses on understanding the foundation's funding sources and donor behavior.

### Key KPIs

- Total Donors — 250
- Total Donation — ₹796.81M
- Average Donation — ₹3.19M
- Count of Donations — 12K
- Donation YTD — ₹200.63M

### Key Analysis

- Top 10 Donors
- Number of Donors by City
- Donor Contribution vs Donor Frequency
- Average Donation by Category

### Business Questions

- Who are the foundation's largest contributors?
- Which cities have the highest number of donors?
- Which donor category has the highest average contribution?
- How does donation frequency relate to total contribution?
- Is the foundation heavily dependent on a small group of major donors?

---

## 03 — Scholarship Distribution

The Scholarship Distribution page focuses on where scholarship funds are being distributed and where pending amounts remain.

### Key KPIs

- Total Universities — 10
- Total Institutes — 15
- Students Supported — 2.00K
- Distributed Scholarship — ₹76.96M
- Pending Scholarship — ₹4.52M

### Key Analysis

- Scholarship Distribution Trend
- Scholarship Distribution by Institute
- Scholarship Distribution by University
- Pending Scholarship by Institute
- Distributed Scholarship by Private vs Public Institutions

### Business Questions

- How does scholarship distribution change over time?
- Which institutes receive the highest scholarship amounts?
- Which universities receive the most financial support?
- Which institutes have the highest pending scholarship amounts?
- How is scholarship funding distributed between public and private institutions?

---

## 04 — Student Analysis

The Student Analysis page focuses on understanding the students receiving educational support.

### Key KPIs

- Total Students — 2.00K
- Student Supported — 2.00K
- Male Students — 1K
- Female Students — 888
- Average Family Income — ₹203.49K

### Key Analysis

- Student Supported by City
- Student Distribution by Course
- Student Distribution by Academic Performance
- Students by Academic Performance
- Students by Family Income Range
- Student Supported by Gender

### Business Questions

- Which cities have the highest number of supported students?
- Which courses are most commonly pursued by scholarship recipients?
- What is the academic performance profile of supported students?
- What is the family income profile of students?
- How are students distributed by gender?
- Are scholarships reaching students from financially weaker backgrounds?

---

# Key Business Questions

The dashboard is designed to answer four major areas of the foundation's operations.

### Funding

1. Who are the foundation's most valuable donors?
2. Which donor categories contribute the most?
3. Which cities have the highest number of donors?
4. How does donor contribution compare with donation frequency?

### Scholarship Distribution

5. Which universities and institutes receive the most scholarship funding?
6. How does scholarship distribution change over time?
7. Which institutes have the highest pending scholarship amounts?
8. How is scholarship funding distributed between public and private institutions?

### Student Support

9. Which cities have the highest number of supported students?
10. Which courses are most common among scholarship recipients?
11. What is the academic performance profile of supported students?
12. What is the family income profile of supported students?
13. What is the gender distribution of supported students?

### Overall Impact

14. How much funding is coming into the foundation?
15. How much scholarship funding is being distributed?
16. How does donor funding connect to the foundation's educational support?

---

# Data Model

The project follows a structured dimensional data model rather than keeping all information in a single flat table.

### Dimension Tables

- `Dim_City`
- `Dim_University`
- `Dim_Institute`
- `Dim_Student`
- `Dim_Donor`
- `Date Table`

### Fact Tables

- `Fact_Donation`
- `Fact_Scholarship`
- `Fact_Allocation`

The model connects donors, donations, scholarship distributions, students, universities, institutes, and cities to support interactive analysis across the report.

---

# Dashboard Navigation

The report contains four analytical pages:

```text
Foundation Overview
        ↓
Donor Analysis
        ↓
Scholarship Distribution
        ↓
Student Analysis
