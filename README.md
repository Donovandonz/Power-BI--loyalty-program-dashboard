# Power-BI--loyalty-program-dashboard
✈️ Flight Loyalty Program Analysis 

## Dataset used
-<a href="https://github.com/Donovandonz/Power-BI--loyalty-program-dashboard/blob/main/Customer%20Flight%20Activity.csv">RAW.customer-flight-activity</a>

-<a href="https://github.com/Donovandonz/Power-BI--loyalty-program-dashboard/blob/main/Customer%20Loyalty%20History.csv">RAW.customer-loyalty-history</a>

-<a href="https://github.com/Donovandonz/Power-BI--loyalty-program-dashboard/blob/main/Calendar.csv">RAW.calendar</a>

---

## 🎯 Project Overview

This project analyzes a flight loyalty program with **16,737 total members**, **14.67K active members**, and tracks key performance indicators including Customer Lifetime Value (CLV), churn rate, points economics, and member behavior patterns.

---

## 🛠️ Tools Used

| Tool | Purpose |
|------|---------|
| **📗 Excel** | Data cleaning, transformation, and initial exploration |
| **📊 Power BI** | Interactive dashboard creation, DAX calculations, and visualization |

---

### Key Metrics at a Glance
| Metric | Value |
|--------|-------|
| **Total Members** | 16,737 |
| **Active Members** | 14,670 |
| **Average CLV** | $7,990 |
| **Churn Rate** | 12.35% |
| **Total Points Earned (2017-2018)** | 796.5M |
| **Total Points Redeemed** | 12.3M |
| **Redemption Rate** | 1.5% |

---

## 📈 Analysis Modules (Dashboard pages)

### 1. Executive Summary Dashboard
- High-level KPIs and metrics
- Member growth trends
- Program performance overview

### 2. Member Behavior Analysis
- Segmentation by loyalty card (Aurora, Nova, Star)
- Demographics breakdown (marital status, education, gender)
- Flight frequency patterns
- Points earning behavior

### 3. Retention & Churn Analysis
- Churn rate tracking (12.35%)
- Member lifetime analysis
- Cancellation patterns
- Risk factor identification

### 4. Points Economics
- Points earning vs. redemption analysis
- Redemption rate trends (1.5% overall)
- Points liability management
- Cost analysis by enrollment year

### 5. Geographic Analysis
- Provincial distribution
- Top performing regions
- CLV by province
- Regional opportunities

## 🔍 Key Insights

### Member Demographics
- **Marital Status**: Married, Single, Divorced 
- **Loyalty Card Distribution**: Aurora, Nova, Star segments
- **Education Levels**: Bachelor, Doctorate, etc.

### Top Performing Members
The top member (ID: 689839) earned **268,287 points** across 90 flights with an average of **2,085 points per flight**.

### Geographic Highlights
- **Ontario** leads in total flights and CLV
- **British Columbia** shows strong member activity
- **Prince Edward Island** has lowest member count but potential for growth

### Points Economics
- Total points earned (2017-2018): **796.5M**
- Total points redeemed: **12.3M**
- Redemption rate: **1.5%** (opportunity for improvement)

---

## 📊 Power BI Dashboards

The project includes 5 interactive Power BI dashboards:

| Dashboard | Description |
|-----------|-------------|
| **Executive Summary** | High-level KPIs and program performance |
| **Member Behavior** | Demographics, segmentation, flight patterns |
| **Retention & Churn** | Churn analysis, member lifetime |
| **Points Economics** | Points earning, redemption, liability |
| **Geographic Analysis** | Provincial distribution, regional CLV |

---

## 💡 Insights & Recommendations

1. **Increase Redemption Rate** (currently only 1.5%)
2. **Target High-Value Segments** (Nova and Star card holders)
3. **Geographic Expansion** in underperforming provinces
4. **Churn Reduction Strategies** for at-risk members
5. **Points Optimization** to improve engagement

---

# Flight Loyalty Program - Data Dictionary

## Member Demographics Table
| Field | Description | Data Type | Example |
|-------|-------------|-----------|---------|
| Loyalty Number | Unique member identifier | Integer | 689839 |
| Loyalty Card | Card tier (Aurora/Nova/Star) | String | Nova |
| City | Member's city | String | Vancouver |
| Province | Member's province | String | British Columbia |
| Marital Status | Married/Single/Divorced | String | Married |
| Education | Education level | String | Bachelor |
| Gender | Male/Female | String | Female |
| Enrollment Type | Standard/Promotion | String | Standard |
| Enrollment Year | Year of enrollment | Integer | 2017 |

## Flight Activity Table
| Field | Description | Data Type | Example |
|-------|-------------|-----------|---------|
| Loyalty Number | Member identifier | Integer | 689839 |
| Year | Flight year | Integer | 2017 |
| Month | Flight month | Integer | 5 |
| Total Flights | Number of flights | Integer | 90 |
| Total Points Earned | Points accumulated | Float | 268,287.00 |
| Avg Points Per Flight | Points per flight avg | Float | 2,085.27 |

## Points Transactions Table
| Field | Description | Data Type | Example |
|-------|-------------|-----------|---------|
| Year | Transaction year | Integer | 2017 |
| Total Points Earned | Annual points earned | Float | 334,315,730.00 |
| Total Points Redeemed | Annual points redeemed | Float | 5,633,888 |
| Points Net | Net points balance | Float | 328,681,842.00 |
| Redemption Rate | Redeemed/Earned % | Percentage | 1.7% |

## Customer Lifetime Value (CLV) Table
| Field | Description | Data Type | Example |
|-------|-------------|-----------|---------|
| Loyalty Number | Member identifier | Integer | 689839 |
| Sum of CLV | Total CLV value | Float | 8,460.81 |
| Member Status | Active/Cancelled | String | Active |
| Cancellation Date | If cancelled | Date | 2018-06-15 |

## Key Performance Indicators (KPIs)
| KPI | Definition | Current Value |
|-----|------------|---------------|
| Total Members | Count of unique members | 16,737 |
| Active Members | Members with activity in last 12 months | 14,670 |
| Average CLV | Mean customer lifetime value | $7,990 |
| Churn Rate | % of members cancelled | 12.35% |
| Redemption Rate | Points redeemed / Points earned | 1.5% |
| Points per Flight | Avg points earned per flight | Varies by card |


---
## Insights

## 🎯 Member Demographics

### Marital Status Distribution
| Status | Total Members | % of Total | Active Members | Active Rate |
|--------|---------------|------------|-----------------|-------------|
| **Married** | 9,735 | 58.2% | 8,520 | 87.5% |
| **Single** | 4,484 | 26.8% | 3,920 | 87.4% |
| **Divorced** | 2,518 | 15.0% | 2,230 | 88.6% |
| **TOTAL** | **16,737** | **100%** | **14,670** | **87.7%** |

*Insight: Married members make up the largest segment (58.2%) with strong active rates. Divorced members show the highest active rate (88.6%), indicating strong engagement.*

### Member Status Breakdown
- **Active Members**: 14,670 (87.7% of total)
  - Married: 8,520 (58.1% of active)
  - Single: 3,920 (26.7% of active)
  - Divorced: 2,230 (15.2% of active)
  
- **Inactive/Cancelled Members**: 2,067 (12.3% of total)
  - Married: 1,215 (58.8% of inactive)
  - Single: 564 (27.3% of inactive)
  - Divorced: 288 (13.9% of inactive)

### Active Rate by Marital Status
| Status | Active Rate | Comparison to Average |
|--------|-------------|----------------------|
| Divorced | 88.6% | ▲ +0.9% |
| Married | 87.5% | ▼ -0.2% |
| Single | 87.4% | ▼ -0.3% |
| **Overall** | **87.7%** | **Baseline** |


---

## 🎯 Targeted Recommendations by Marital Status

### For Married Members (Largest Segment - 9,735 members)
- **Family Package Deals**: Create bundled offers for family travel
- **Anniversary/Date Night Promotions**: Special points for couple travel
- **School Holiday Programs**: Target during school breaks
- **Potential**: 58% of membership base, strong engagement potential

### For Single Members (26.8% of membership - 4,484 members)
- **Solo Traveler Benefits**: No single supplements, solo traveler lounges
- **Weekend Getaway Packages**: Target short trips
- **Social Flight Events**: Create community experiences
- **Potential**: Growing segment with 87.4% active rate

### For Divorced Members (Highest Active Rate - 88.6%)
- **"New Beginnings" Campaigns**: Target lifestyle changes
- **Solo Adventure Packages**: Curated solo travel experiences
- **Flexible Booking Options**: Cater to changing schedules
- **Potential**: Most engaged segment despite smallest size

### Active Rate Comparison
| Segment | Active Rate | Engagement Level |
|---------|-------------|------------------|
| Divorced | 88.6% | ⭐⭐⭐ HIGHEST |
| Married | 87.5% | ⭐⭐ HIGH |
| Single | 87.4% | ⭐⭐ HIGH |

---

## Marital Status Distribution
The analysis revealed a clear segmentation pattern:

**Married (58.2% - 9,735 members)**
- Largest segment by far
- 8,520 active members (87.5% active rate)
- Primary target for family-oriented benefits
- Highest potential for multi-passenger bookings

**Single (26.8% - 4,484 members)**
- Second largest segment
- 3,920 active members (87.4% active rate)
- Key target for solo traveler benefits
- High potential for leisure travel

**Divorced (15.0% - 2,518 members)**
- Smallest but most engaged segment
- 2,230 active members (88.6% active rate - HIGHEST!)
- Opportunity for "fresh start" marketing
- Potential for flexible travel packages

### Key Insight
The divorced segment, despite being the smallest, shows the highest engagement rate (88.6% active), suggesting this group finds exceptional value in the loyalty program. This presents an opportunity for targeted retention campaigns and specialized offerings.

**Key Takeaway**: The 1.5% redemption rate represents both a problem and an opportunity - solving it could transform member engagement and program profitability.

---

## Dashboard overview (Page 1)
-<a href="https://github.com/Donovandonz/Power-BI--loyalty-program-dashboard/blob/main/Executive-summary-dashboard.png">Executive-summary</a>

<img width="1312" height="737" alt="Executive-summary-dashboard" src="https://github.com/user-attachments/assets/a35e92ae-6f51-49b6-ae20-2bfea8dc1136" />

## Dashboard overview (Page 2)
-<a href="https://github.com/Donovandonz/Power-BI--loyalty-program-dashboard/blob/main/Member-behavior-dashboard.png">Member-behavior</a>

<img width="1310" height="737" alt="Member-behavior-dashboard" src="https://github.com/user-attachments/assets/f6fe4f2e-c6bf-41f0-a17b-a0c5a71e475f" />

## Dashboard overview (Page 3)
-<a href="https://github.com/Donovandonz/Power-BI--loyalty-program-dashboard/blob/main/Retention-and-churn-analysis-dashboard.png">Retention-and-churn</a>

<img width="1310" height="738" alt="Retention-and-churn-analysis-dashboard" src="https://github.com/user-attachments/assets/56a94e3e-c73b-449a-b184-d2727732d59d" />

## Dashboard overview (Page 4)
-<a href="https://github.com/Donovandonz/Power-BI--loyalty-program-dashboard/blob/main/Points-economic-dashboard.png">Points-economic</a>

<img width="1310" height="738" alt="Points-economic-dashboard" src="https://github.com/user-attachments/assets/ed5ec17b-e793-4ca6-8ebc-c22ac921e6ba" />

## Dashboard overview (Page 5)
-<a href="https://github.com/Donovandonz/Power-BI--loyalty-program-dashboard/blob/main/Geographic-analysis-dashboard.png">Geographic-analysis</a>

<img width="1311" height="737" alt="Geographic-analysis-dashboard" src="https://github.com/user-attachments/assets/20d76c0f-e5f6-4d19-8e97-ce6fa8e45ee6" />







