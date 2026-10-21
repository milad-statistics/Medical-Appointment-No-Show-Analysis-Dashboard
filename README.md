# Medical Appointment No-Show Analysis Dashboard

## Project Overview

This project analyzes medical appointment attendance data from Brazil using Power BI. The dashboard focuses on understanding no-show patterns, exploring factors associated with missed appointments, and tracking the no-show rate through interactive visualizations.

## Project Objectives

- Analyze patterns in medical appointment no-shows.
- Explore how no-show counts vary across different patient groups.
- Examine no-show patterns by month, age group, and neighborhood.
- Build an interactive dashboard to monitor the no-show rate and number of missed appointments.

## Dataset

**Dataset:** Medical Appointment No Shows  
**Source:** [Kaggle – Medical Appointment No Shows](https://www.kaggle.com/datasets/joniarroba/noshowappointments)

The dataset contains information about medical appointments, including patient demographics, appointment dates, health conditions, scholarship status, SMS reminders, and appointment attendance status.

## Tools Used

- **Power BI** – Dashboard development and interactive data visualization
- **Power Query** – Data cleaning and transformation
- **DAX** – Measures and calculated columns

## Data Preparation

The following data preparation steps were performed in Power Query:

- Changed column data types where necessary.
- Removed rows containing negative age values.
- Removed duplicate rows.
- Converted patient and appointment identifiers to text.
- Standardized gender values from `M` and `F` to `Male` and `Female`.
- Removed the time component from the appointment date.
- Converted binary values into readable `Yes` and `No` labels for relevant columns.
- Created age groups to support comparisons across different age ranges.

## Dashboard Features

### Key Performance Indicators (KPIs)

- **No-Show Rate:** Percentage of appointments marked as no-shows among the selected appointments.
- **No-Show Count:** Number of appointments marked as no-shows under the current filter context.

### Visualizations

- **Monthly No-Show Count:** A line chart showing changes in no-show counts across months.
- **Top 5 No-Show Neighborhoods:** A bar chart highlighting the five neighborhoods with the highest no-show counts.
- **No-Show Count by Age Group:** A chart comparing no-show counts across age groups.

### Interactive Filters

The dashboard includes slicers for:

- Gender
- Scholarship
- Hypertension
- Diabetes
- Alcoholism
- SMS Received
- No-show Status

A **Reset Filters** button allows users to return to the default dashboard view.

The KPI cards and visualizations respond to filter selections, allowing users to explore different patient groups and combinations of factors.

## Key Analytical Considerations

- No-show counts and no-show rates measure different things. Counts indicate volume, while rates account for the total number of appointments in each group.
- Neighborhoods with more no-shows do not necessarily have higher no-show rates.
- Differences between appointments with and without SMS reminders should be interpreted as associations, not proof of causation.

## Project Outcome

The final dashboard provides an interactive overview of medical appointment no-shows, making it easier to explore monthly patterns and differences across patient demographics, health conditions, and other appointment-related factors.

This project demonstrates practical skills in data preparation, DAX calculations, data visualization, and interactive dashboard development using Power BI.
