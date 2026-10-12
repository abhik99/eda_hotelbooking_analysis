# 🏨 Hotel Booking Demand EDA & Revenue Strategy

[![Python](https://img.shields.io/badge/Python-3.9%2B-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://python.org)
[![EDA](https://img.shields.io/badge/Analysis-Exploratory%20Data%20Analysis-orange?style=for-the-badge)](https://pandas.pydata.org)
[![Pandas](https://img.shields.io/badge/Pandas-Data%20Wrangling-150458?style=for-the-badge&logo=pandas&logoColor=white)](https://pandas.pydata.org)
[![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-11557c?style=for-the-badge)](https://matplotlib.org)
[![Seaborn](https://img.shields.io/badge/Seaborn-Statistical%20Plots-4c72b0?style=for-the-badge)](https://seaborn.pydata.org)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge)](LICENSE)

An in-depth exploratory data analysis and revenue management study conducted on 119,390 hotel booking records spanning City Hotels and Resort Hotels. Investigates cancellation drivers, lead-time dynamics, Average Daily Rate (ADR) seasonality, customer distribution channels, and optimal booking windows to formulate data-backed revenue strategies.

---

## 📌 Table of Contents
- [Executive Summary](#-executive-summary)
- [Dataset Overview](#-dataset-overview)
- [Key Exploratory Insights](#-key-exploratory-insights)
- [ADR Seasonality & Revenue Opportunities](#-adr-seasonality--revenue-opportunities)
- [Cancellation Risk Analysis](#-cancellation-risk-analysis)
- [Strategic Business Recommendations](#-strategic-business-recommendations)
- [Repository Structure](#-repository-structure)
- [Getting Started](#-getting-started)
- [Author & Connect](#-author--connect)

---

## 🚀 Executive Summary
Revenue managers and hospitality operators routinely struggle with high cancellation rates (often exceeding 30%) and sub-optimal pricing during shoulder seasons.

This project analyzes the 119,390 reservation records in `Hotel_bookings.csv` to answer critical operational questions:
- What is the relationship between booking lead time and cancellation probability?
- Which room categories generate the highest Average Daily Rate (ADR) relative to booking volume?
- What booking channels and travel agencies drive the highest guest lifetime value?
- How does seasonality impact City Hotels versus Resort Hotels differently?

---

## 📊 Dataset Overview
- **Total Observations:** 119,390 hotel booking records.
- **Hotel Types:** City Hotel (~60% of bookings) vs. Resort Hotel (~40% of bookings).
- **Core Attributes:** `lead_time`, `arrival_date_year`, `arrival_date_month`, `stays_in_weekend_nights`, `stays_in_week_nights`, `adults`, `children`, `meal`, `country`, `market_segment`, `distribution_channel`, `is_canceled`, `adr`, `reserved_room_type`, `assigned_room_type`.

---

## 💡 Key Exploratory Insights
1. **Property Preference:** City Hotels account for ~60% of total bookings, reflecting high corporate and short-stay urban tourism.
2. **Meal Plan Dominance:** Bed & Breakfast (`BB`) is overwhelmingly preferred by over 77% of travelers across both property types.
3. **Distribution Distribution:** Online Travel Agents (OTAs) and Agent 9 represent the largest single booking channel volume.
4. **Lead Time Distribution:** City Hotels exhibit higher median lead times; guests planning longer stays book significantly further in advance.
5. **Room Type Demand vs Revenue:** Room Type `A` represents the highest volume of reservations; however, Room Types `H`, `G`, and `C` command significantly higher ADR.

---

## 📈 ADR Seasonality & Revenue Opportunities
- **Summer Peak:** Resort Hotels experience massive ADR spikes in July and August, while City Hotels demonstrate more consistent year-round ADR with minor spring and autumn business conference surges.
- **Group vs Transient Pricing:** Group bookings yield lower ADR but lower cancellation variance; transient bookings offer higher rate elasticity.

---

## ⚠️ Cancellation Risk Analysis
- **Lead Time Correlation:** Bookings placed over 90 days in advance exhibit substantially higher cancellation rates than bookings made within a 14-day window.
- **Deposit Policy Impact:** Non-refundable deposit requirements were historically concentrated in high-risk segments; however, flexible cancellation policies paired with automated confirmation reminders mitigate no-show losses.

---

## 🎯 Strategic Business Recommendations
- **Inventory Re-allocation:** Hotels should convert or expand Room Types `A` and `H` to capture premium ADR without hurting occupancy.
- **Dynamic Deposit Policies:** Implement progressive deposits for bookings with lead times > 60 days during peak summer months.
- **Direct Booking Incentives:** Offer complimentary breakfast (`BB`) upgrades on direct hotel websites to reduce commission bleed to third-party OTAs.

---

## 📁 Repository Structure
```text
├── Hotel_Booking_Analysis.ipynb  # End-to-end data cleaning, EDA & statistical testing notebook
├── Hotel_bookings.csv            # 119k booking observations dataset
├── Presentation.pptx             # Executive slide deck detailing findings and revenue charts
└── README.md                     # Comprehensive project documentation
```

---

## 🛠️ Getting Started

### 1. Clone the Repository
```bash
git clone https://github.com/abhik99/eda_hotelbooking_analysis.git
cd eda_hotelbooking_analysis
```

### 2. Install Required Packages
```bash
pip install pandas numpy matplotlib seaborn jupyter
```

### 3. Launch Notebook
```bash
jupyter notebook Hotel_Booking_Analysis.ipynb
```

---

## 👨‍💻 Author & Connect

**Abhishek Kumar (Abhi)**  
*Data Scientist & Analytics Engineer*

- 🌐 **Portfolio:** [abhicodes.online](https://abhicodes.online)
- 💼 **LinkedIn:** [linkedin.com/in/abhik99](https://linkedin.com/in/abhik99)
- 🐙 **GitHub:** [@abhik99](https://github.com/abhik99)
- 📧 **Email:** [akdevil27boy@gmail.com](mailto:akdevil27boy@gmail.com)

---
*Distributed under the MIT License.*
