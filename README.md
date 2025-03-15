# call-center-performance-dashboard
# Call Center Insights Dashboard

Welcome to the **Call Center Insights Dashboard** project. This dashboard is designed to provide an interactive and comprehensive view of call center performance, enabling users to monitor key performance indicators (KPIs) and gain valuable insights into operations.

## Overview

The dashboard integrates multiple data sources and provides visualizations for critical metrics including Average Handle Time (AHT), Percentage of Answered Calls (PCA%), Service Level Agreement (SLA%), Customer Satisfaction (CSAT), and First Call Resolution (FCR). With interactive charts, bookmarks, slicers, drill-throughs, and tooltips, users can explore detailed views and trends in call center data.

## Features

- **Key Metrics Calculation & Visualization**
  - **Average Handle Time (AHT):** Computed as Total Handle Time divided by Answered Calls.
  - **Percentage of Answered Calls (PCA%):** (Answered Calls / Offered Calls) * 100.
  - **Service Level Agreement (SLA%):** (Answered Calls Within Service Level / Offered Calls).

- **Interactive Charts**
  - **Average Offered Calls Per Day:** Trend analysis of offered calls on a daily basis.
  - **Offered Calls by Day of the Week:** Visualization of average offered calls across each day.
  - **Total Offered Calls Per Skill (Monthly View):** Monthly breakdown by skill.
  - **AHT Per Language (Quarterly):** Performance comparison across different languages for each quarter.
  - **Percentage of Answered Calls per Skill:** Insight into performance metrics by skill.
  - **AHT Comparison for AR & ENG Teams:** A boxplot chart comparing AHT between AR and ENG teams with descriptive insights.
  - **CSAT & FCR Relationship:** Chart showing the relationship between customer satisfaction and first call resolution scores.

## Data Model

The dashboard is built upon a robust data model where:

- **Calls Table:** Contains detailed call records including times, call outcomes, and performance measures.
- **CSAT Table:** Includes customer satisfaction scores (scored from 1 to 5, where Very Satisfied = 5 and Very Dissatisfied = 1).
- **Calendar Table:** Acts as a central date dimension, linking both the Calls and CSAT tables for time-based analysis.

## Call Center Calculations

The following metrics are calculated to evaluate call center performance:

| **Metric**                          | **Calculation**                                                       |
|-------------------------------------|-----------------------------------------------------------------------|
| **Answered Calls**                  | Ans Calls Within Service Level + Ans Calls After Service Level        |
| **Total Handle Time (THT)**         | Talk Time + Hold Time + ACW Time                                      |
| **Average Handle Time (AHT)**       | THT / Answered Calls                                                  |
| **Service Level Agreement (SLA)**   | Ans Calls Within Service Level / Offered Calls                        |
| **Percentage of Answered Calls (PCA%)** | (Ans Calls / Offered Calls) * 100                                  |
| **CSAT**                            | Average scores (Very Satisfied = 5 & Very Dissatisfied = 1)             |
| **FCR**                             | Average scores (Yes = 1 & No = 0)                                       |

## Dashboard Design & Evaluation Criteria

- **Design & Format**
  - Purposeful theme and color scheme.
  - Clear, concise labels and aligned charts.
  - Consistent formatting across all visual elements.

- **Interactivity**
  - Use of bookmarks, slicers, drill-throughs, and tooltips to enhance user experience.
  - Detailed insights and comments accompanying the visualizations.

- **Insights & Value**
  - Each chart and metric is complemented by descriptive insights.
  - Comparisons and analyses (e.g., boxplot for AR vs. ENG teams) provide actionable feedback.

## Dashboard Preview

Below is an image of the dashboard design. Replace the placeholder image with your actual dashboard image.

![Dashboard Preview](dashboard.png)


