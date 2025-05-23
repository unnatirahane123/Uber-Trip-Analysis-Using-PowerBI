# 🚖 Uber Trip Analysis | Power BI Dashboard

A comprehensive Power BI solution to analyze Uber trip data and uncover trends in trip efficiency, booking behavior, vehicle preference, and geographic demand.

---

## 🧠 Business Requirement

**Goal:**  
To analyze Uber trip data using Power BI and provide actionable insights into booking trends, revenue generation, trip efficiency, and customer preferences.

---

## 📊 Dashboards Overview

### 📌 Dashboard 1: Overview Analysis

**Key Objectives:**
- Analyze total bookings, booking value, trip distance, and average trip time.
- Identify popular payment types and trip types (day/night).
- Understand high-performing locations and vehicles.

**KPI Metrics:**
- ✅ Total Bookings
- ✅ Total Booking Value
- ✅ Average Booking Value
- ✅ Total Trip Distance
- ✅ Average Trip Distance
- ✅ Average Trip Time

**Features & Enhancements:**
- Dynamic Measure Selector (Bookings, Revenue, Distance)
- Filters by City & Date
- Dynamic Titles
- Conditional Formatting on Grid
- Tooltips for insights like Avg Distance & Value
- Clear Slicer Button
- Raw Data Export Button

**Visuals:**
- Donut charts by Payment Type and Trip Type
- Booking trends by Day
- Top Pickup & Drop-off Locations
- Vehicle-wise KPI Table
- Most Preferred Vehicle by Pickup Location
- Farthest Trip Details

![Overview Dashboard](images/overview_dashboard.png)

---

### ⏱ Dashboard 2: Time Analysis

**Objective:**  
Understand ride demand across different **times of day and days of the week** to optimize operations, driver deployment, and pricing strategies.

**Global Dynamic Measure (applies to all visuals):**
- ✔ Total Bookings
- ✔ Total Booking Value
- ✔ Total Trip Distance

**Visualizations:**
- **Area Chart** by Pickup Time (10-minute intervals)
- **Line Chart** by Day Name (Mon–Sun)
- **Heatmap** (Matrix) – Hour (0–23) × Day (Mon–Sun) with measure value

**Key Insights:**
- Detect peak & off-peak hours
- Understand weekday vs weekend demand
- Plan promotions or incentives during low traffic hours

![Time Analysis Dashboard](images/time_analysis_dashboard.png)

---

### 📋 Dashboard 3: Details Tab

**Purpose:**  
Provide granular visibility into every trip record and allow users to drill through from summary visuals to raw data.

**Features:**
- Grid Table showing:
  - Trip ID
  - Pickup Time & Hour
  - Vehicle Type
  - Payment Method
  - Passenger Count
  - Trip Distance
  - Booking Value
  - Pickup & Drop-off Locations
- **Drill-through** from charts to view detailed records
- **Bookmark** toggle to switch between full dataset view and filtered detail

![Details Dashboard](images/details_dashboard.png)

---

## 🧰 Technology Stack

| Tool            | Usage                     |
|-----------------|---------------------------|
| Power BI        | Data modeling, dashboard   |
| Python (optional) | Data cleaning, preprocessing |
| SQL (optional)    | Querying structured data |
| Power Automate (optional) | Raw data export |

---

## 📦 Dataset Overview

### 📁 Trip Details Table

| Column          | Description                     |
|------------------|---------------------------------|
| Trip ID          | Unique trip identifier          |
| Pickup Time      | Timestamp when trip started     |
| Dropoff Time     | Timestamp when trip ended       |
| Passenger Count  | Number of passengers            |
| Trip Distance    | Miles traveled                  |
| Payment Type     | Cash, Uber Pay, etc.            |

### 📁 Location Table

| Column       | Description              |
|--------------|--------------------------|
| Location ID  | Unique ID of area        |
| Area Name    | Pickup or drop location  |
| City         | City name                |

---

## 📈 Expected Outcomes

✔ Identify high/low demand periods  
✔ Optimize vehicle distribution by time and location  
✔ Enhance pricing strategy based on trends  
✔ Analyze trip efficiency and customer behavior  
✔ Improve user experience with drill-through and raw data export

---

## ▶️ How to Run the Project

1. **Install Power BI Desktop**:  
   [Download Power BI Desktop](https://powerbi.microsoft.com/en-us/desktop/)

2. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/uber-trip-analysis.git

