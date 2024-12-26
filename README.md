# Power BI Dashboard for Tracking Student Progress and Performance

## Project Overview

This project involves creating a Power BI dashboard for **Global Careers**, an organization that provides training in Power BI and AWS Cloud. The goal is to effectively monitor the progress and performance of students through a comprehensive dashboard that tracks key metrics such as attendance, participation, assessments, and learner status.

## Key Objectives

1. **Visualize Learner Performance Metrics:**

   - Graduation, certification, and dropout rates.
   - Average attendance, participation, and assessment scores.

2. **Provide Detailed Insights:**

   - Individual learner progress and engagement.
   - Support trainers and program managers in identifying learners at risk.

3. **Enhance Data Exploration:**
   - Interactive slicers for cohort, track, certification type, and learner status.

## Features

### 1. Dashboard Components

- **Page 1: Overall Performance Metrics**

  - Visualizations:
    - Bar charts for graduation rates, certification rates, dropout rates, and average metrics.
    - Summary cards for total certifications, learners, dropouts, and graduations.
  - Filters:
    - By cohort, track, certification type, and learner status.

- **Page 2: Detailed Learner Insights**
  - Visualizations:
    - Table of learners with key metrics.
    - Summary cards for labs completed, hours spent in class, and average rates.
  - Filters:
    - By cohort, track, month, week, and program status.

### 2. Data Preparation

Multiple files with data in them were loaded from the following folder structure. Data cleaning involved loading these files, appending records across weeks, and ensuring consistent formats for subsequent analysis.

#### Folder Structure:

```plaintext
data/
├── Cloud Training/
│   ├── Labs & Quizzes/
│   │   ├── labs_and_quizzes.xlsx
│   ├── Participation/
│   │   ├── AWS.xlsx
│   ├── Status of Learners/
│   │   ├── participant_status.xlsx
│   ├── Zoom Attendance/
│   │   ├── Week 1/
│   │   │   ├── 05-Aug-2024.csv
│   │   │   ├── 06-Aug-2024.csv
│   │   │   ├── 07-Aug-2024.csv
│   │   │   ├── 08-Aug-2024.csv
│   │   │   ├── 09-Aug-2024.csv
│   │   ├── Week 2/
│   │   ├── Week 3/
│   │   ├── Week 4/
│   │   ├── Week 5/
│   │   ├── Week 6/
│   │   ├── Week 7/
│   │   ├── Week 8/
│   │   ├── Week 9/
│   │   ├── Week 10/
├── PowerBI Training/
│   ├── Labs & Quizzes/
│   │   ├── labs_and_quizzes.xlsx
│   ├── Participation/
│   │   ├── PowerBI.xlsx
│   ├── Status of Learners/
│   │   ├── participant_status.xlsx
│   ├── Zoom Attendance/
│   │   ├── Week 1/
│   │   │   ├── 05-Aug-2024.csv
│   │   │   ├── 06-Aug-2024.csv
│   │   │   ├── 07-Aug-2024.csv
│   │   │   ├── 08-Aug-2024.csv
│   │   │   ├── 09-Aug-2024.csv
│   │   ├── Week 2/
│   │   ├── Week 3/
│   │   ├── Week 4/
│   │   ├── Week 5/
│   │   ├── Week 6/
│   │   ├── Week 7/
│   │   ├── Week 8/
│   │   ├── Week 9/
│   │   ├── Week 10/

```

### 3. Data Modeling and DAX

- **Modeling:** With the help of Power BI model view, I explicitly established relationships between related tables.
- **DAX Formulas:**
  - Dynamic calculations for averages and rates.
  - Filtering metrics by various dimensions.

### 4. Attendance Calculation

A learner is marked "attended" if they spent more than **30 minutes** in a Zoom session.

## Challenges and Learnings

- **Nested Folder Structure:**
  - Navigating and loading deeply nested directories was initially challenging. Ensuring correct appending and querying across multiple files was a key learning area.
- **Data Cleaning:**
  - Standardizing formats for attendance and performance data required significant effort.
- **New Tools and Techniques:**
  - Leveraged DAX for dynamic calculations and slicers for interactivity.
- **Unpivoting Data:**
  - Learned how unpivoting data can simplify aggregations, particularly for labs and quizzes.

## Conclusion

This dashboard provides an essential tool for tracking learner progress and engagement, offering insights into program effectiveness and helping stakeholders make informed decisions.

## License

This project is for educational purposes as part of the Labs for the Data Analytics and Visualization with Power BI.

---

Feel free to modify the folder structure or other details as needed!
