## Hotel Booking Analysis & Dashboard

## Project Overview
This project focuses on analyzing hotel booking data to understand cancellation behavior, lead time impact, and revenue trends.

Along with Exploratory Data Analysis (EDA), an interactive dashboard is built using Microsoft Power BI to visualize key business metrics and support data-driven decision-making.

The goal is to help hotels reduce cancellations, optimize pricing, and improve operational efficiency.

## Objectives
Analyze the relationship between lead time and cancellations

Identify patterns to predict booking cancellations

Build an interactive dashboard for real-time insights

Suggest strategies to maximize revenue and occupancy

Improve customer experience and hotel operations

## Dataset Details
Source: Hotel Booking Dataset

Rows: 119,390

Columns: 32

## Key Variables:
Column	Description

hotel	Hotel type (Resort/City)

is_canceled	1 = canceled, 0 = not canceled

lead_time	Days between booking and arrival

adr	Average Daily Rate

adults, children, babies	Number of guests

customer_type	Type of customer

market_segment	Booking source

deposit_type	Deposit category

reservation_status	Booking status

## Data Cleaning & Feature Engineering
Filled missing values:

children → 0

country → 'others'

agent → 0

Dropped column:

company (high missing values)

Removed invalid records:

total_people = 0

Created new features:

total_people = adults + children + babies

total_stay = stays_in_weekend_nights + stays_in_week_nights

## Key Insights
## 1. Seasonal Trends
Peak bookings observed during summer & winter seasons

Helps in dynamic pricing and promotional planning

## 2. Lead Time vs Cancellations
Longer lead time → higher cancellation probability

Short lead-time bookings are more reliable

## 3. Customer Behavior
Majority customers are transient (leisure travelers)

Useful for targeted marketing campaigns

## 4. Revenue Insights
Higher ADR (Average Daily Rate) linked with longer lead time

Strong relationship between pricing, lead time, and cancellations

## 5. Operational Strategy
Implement controlled overbooking

Optimize staffing and resource allocation

## Dashboard (Power BI)
An interactive dashboard was developed using Microsoft Power BI to provide real-time business insights.

## Dashboard Features:
## KPI Cards:

Total Bookings

Cancellation Rate

Average ADR

Total Revenue

## Visualizations:

Lead Time vs Cancellation trend

Monthly booking trends

Revenue distribution by hotel type

Customer segmentation analysis

## Filters / Slicers:

Hotel Type

Customer Type

Market Segment

Date Range

## Key Benefit:
The dashboard enables stakeholders to quickly identify trends, monitor performance, and make data-driven decisions.

## Tools & Technologies
Python: pandas, numpy, matplotlib, seaborn, plotly

Visualization: Microsoft Power BI

Environment: Google Colab

## Visualizations (EDA)
Univariate Analysis: Histograms, Pie Charts

Bivariate Analysis: Boxplots, Scatter Plots

Multivariate Analysis: Correlation Heatmaps

## 20+ meaningful charts created using UBM (Univariate, Bivariate, Multivariate) approach

## Business Impact
 Reduce booking cancellations

 Improve revenue management strategies

 Enable data-driven decision making

 Enhance customer experience

 Optimize hotel operations

## Conclusion
This project demonstrates how combining data analysis + interactive dashboarding can solve real-world business problems in the hospitality industry.

It highlights the importance of lead time, pricing strategies, and customer behavior analysis in improving hotel performance.
