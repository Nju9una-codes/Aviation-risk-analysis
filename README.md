#  Aviation Risk Analysis

##  Objective

This project analyzes historical aviation accident data to identify safer aircraft makes and models. The goal is to provide data-driven recommendations for aircraft acquisition, targeting reduced accident and fatality rates.

---

##  Business Context

Our team is evaluating the possibility of entering the aviation industry for private and commercial operations. To minimize risk and make sound investments, we need to understand:

- Which aircraft types are involved in fewer fatal incidents?
- What patterns emerge over time or across geographic regions?
- Are there specific manufacturers with consistently safer records?

---

##  Problem Statement

Given historical aviation accident data, determine which aircraft types pose the least risk. Use this insight to guide purchasing and strategic planning decisions.

---

##  Dataset Overview

- **Source:** National Transportation Safety Board (NTSB)
- **Years Covered:** 1962–2023
- **Records:** Over 90,000
- **Key Features:** 
  - Make & Model
  - Event Date
  - State
  - Injury Severity (Fatal, Serious, Minor, None)
  - Number of Injuries (Pilots, Crew, Passengers)

---

##  Data Preparation Steps

- Converted `Event Date` into `Year`
- Handled missing values by imputing or dropping where necessary
- Created a new `Total Involved` metric summing all injury columns
- Filtered out null aircraft make/model records
- Grouped rarely occurring aircraft under “Other”
- Standardized severity categories

---

## 🧪 Exploratory Data Analysis Highlights

### 1. **Fatal Injuries by Country**
- A bar chart was used to display fatal injuries aggregated by country.
- The U.S. had the highest total, due to both population and data source origin.
- This view helps assess where most fatal incidents are occurring.

### 2. **Accidents Over Time**
- A line graph showing the total number of reported accidents by year.
- Accidents peaked in the 1980s and have declined since.
- Indicates potential improvement in aviation safety over time.

### 3. **Reported Accidents by Flight Purpose**
- Visualized flight types involved in accidents (e.g., Personal, Business, Instructional).
- Personal-use flights had the highest number of reported accidents.
- Insight: Private flying has more variability and may require more safety focus.

### 4. **Top 10 Aircraft Makes in Reported Accidents**
- A horizontal bar graph showing makes with the highest accident count.
- Cessna and Piper were frequent, likely due to higher usage.
- Normalization by usage would improve this insight (pending operational data).

---

##  Tableau Dashboard

The interactive dashboard includes:

- **US Map**: Fatal Injuries by State
- **Line Chart**: Yearly accident trends
- **Pie Chart**: Injury severity distribution
- **Bar Chart**: Top aircraft involved in fatal incidents

>  Downloaded as PDF and submitted per Flatiron requirements.

---

## Repository Contents

| File | Description |
|------|-------------|
| `notebook.ipynb` | The full Jupyter notebook with analysis and visuals |
| `presentation.pdf` | Project presentation in slide format |
| `dashboard.pdf` | Exported Tableau visual dashboard |
| `README.md` | Project overview and documentation |

---

## Recommendations

- Favor aircraft types with consistently lower fatal accident rates (e.g., newer Cessna models).
- Avoid high-risk aircraft identified in the dashboard.
- Use seasonal trends to improve planning and reduce risk.
- Consider including pilot experience, weather, and flight hours in future analyses.

---

## Next Steps

- Normalize fatality rates using number of flights per aircraft type (if data becomes available)
- Enrich dataset with pilot logbooks or FAA maintenance records
- Deploy interactive Tableau dashboards to management team

---

## 👤 About Me

**Name:** Patrick Maina  
**Email:** mpatricknjuguna02@gmail.com  


---

