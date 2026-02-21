#  Hotel Booking Analysis: Lead Time & Cancellations

##  Project Overview

Hotels face revenue loss due to booking cancellations, especially for reservations made well in advance. This project explores **how lead time affects cancellations** and identifies patterns to help hotels **optimize revenue** and **enhance guest experience**.

Using **Exploratory Data Analysis (EDA)** and regression, this project provides actionable insights for **revenue management, operational planning, and marketing strategies**.

---

## Objectives

- Analyze the effect of **lead time** on booking cancellations.  
- Identify trends and patterns to **predict cancellations**.  
- Suggest strategies to **reduce cancellations** and **maximize revenue**.  
- Improve **guest satisfaction** and operational efficiency.  

---

## Dataset Details

- **Source:** Hotel Booking Dataset  
- **Rows:** 119,390  
- **Columns:** 32  

**Key Variables:**

| Column | Description |
|--------|-------------|
| `hotel` | Hotel type (Resort/City) |
| `is_canceled` | 1 = canceled, 0 = not canceled |
| `lead_time` | Days between booking and arrival |
| `adr` | Average Daily Rate |
| `adults`, `children`, `babies` | Number of guests |
| `customer_type` | Customer type (Transient/Group/Contract) |
| `market_segment` | Source of booking |
| `deposit_type` | Type of deposit |
| `reservation_status` | Current booking status |

**Data Cleaning & Feature Engineering:**

- Filled missing values: `children → 0`, `country → 'others'`, `agent → 0`  
- Dropped column `company` (too many nulls)  
- Removed bookings with `total_people = 0`  
- Added new features:  
  - `total_people = adults + children + babies`  
  - `total_stay = stays_in_weekend_nights + stays_in_week_nights`  

---

##  Key Insights

1. **Seasonal Trends:**  
   - High bookings during summer & winter months  
   - Hotels can plan promotions and pricing accordingly  

2. **Lead Time & Cancellations:**  
   - Longer lead time → higher cancellation probability  
   - Short lead-time bookings are more reliable for revenue planning  

3. **Guest Composition:**  
   - Majority are leisure or transient customers  
   - Helps in **targeted marketing** strategies  

4. **Revenue Analysis:**  
   - ADR increases with longer lead time  
   - Correlation exists between ADR, lead time, and cancellations  

5. **Operational Recommendations:**  
   - Use **overbooking strategies** for high-cancellation periods  
   - Plan staffing and resources based on cancellation trends  

---

##  Tools & Libraries

- **Python Libraries:** pandas, numpy, matplotlib, seaborn, plotly  
- **Environment:** Google Colab  

---

## Visualizations

- **Univariate Analysis:** Histograms, Pie charts  
- **Bivariate Analysis:** Boxplots, Scatter plots  
- **Multivariate Analysis:** Correlation heatmaps, 3D insights  

> 20+ meaningful charts created following UBM (Univariate, Bivariate, Multivariate) approach  

## Business Impact

- Reduce booking cancellations & improve revenue  
- Optimize **pricing strategies** for peak/off-peak seasons  
- Improve **guest experience** by better planning  
- Provide actionable insights for **operational & marketing decisions**  

