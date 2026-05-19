# Centauri Airlines Passenger Satisfaction Dashboard

## Project Overview

This project analyses airline passenger satisfaction data to understand which service areas, passenger segments, and journey factors are associated with overall satisfaction.

The dashboard was built in microsoft excel using functions and formulas focusing on service ratings, passenger experience areas, flight class, age groups, customer loyalty, and overall satisfaction outcomes.

The aim of the project was to identify where Centauri Airlines should focus improvement efforts to increase passenger satisfaction.

![Dashboard Preview](dashboard-preview.png)

---

## Business Question

**What drives passenger satisfaction at Centauri Airlines?**

Supporting questions explored in the dashboard:

- Which passenger experience areas receive the highest and lowest service ratings?
- Do service strengths and weaknesses vary by flight class?
- Which age groups make up the main passenger base?
- How do different age groups rate us?
- How satisfied are passengers overall?
- How strongly is Overall Service Score (OSS) linked to satisfaction?
- Does satisfaction vary by flight class?
- Does loyalty result in satisfaction?

---

## Excel Techniques Used

This project used a formula-driven approach to build the dashboard and support analysis.

Key Excel techniques included:

- `COUNTIF` and `COUNTIFS`
- `AVERAGEIF` and `AVERAGEIFS`
- `SUMIF` and `SUMIFS`
- `IF` and `IFS`
- Ranking formulas - `RANK.EQ`
- Lookup formulas - `XLOOKUP`
- Dynamic Array Functions - `Transpose` , `Unique`, `Sort`
- Data validation dropdowns - ability to choose different flight class.
- Conditional formatting - colour scales for service ratings.
- Fill Series.
- Helper columns - Age bands, Overall Service Score bands, Flight haul bands, Delay bands etc.
- Visualisation techniques 
- Donut charts
- Bar charts
- Line chart
- 100% stacked bar charts
- Dynamic tables 
- Custom number formatting
- Dashboard layout and visual storytelling
- Dashboard Protection
   
---

## Data Preparation and Assumptions

Several helper columns were created to support the analysis:

- **Overall Service Score**: calculated as the average rating across passenger experience areas.
- **Age Group**: passengers were grouped into age bands.
- **Flight Haul Band**: flight distance was grouped into short, medium, long, and very long-haul categories.
- **Delay Band**: flights were grouped according to no delay, minor, moderate and severe delay.
- **Overall Service Score Band**: passengers were grouped based on their overall service score.
- **Satisfaction Flag**: used to calculate satisfaction rates. 1 = Satisfied. 0 = Neutral/Dissatisfied.

Important assumptions:

- Rating values of `0` were treated as **Not Rated / Not Applicable** and excluded from service rating calculations. This is atleast what the inital author of the data assumes.
- Flight distance was treated as miles.
- The analysis focuses on association rather than causation. For example, higher satisfaction on longer-haul flights may be influenced by class mix rather than flight haul alone.

Other information:

- Initial data was very clean and well structured. There were no null/empty values and each row represented a unique passenger meamning no duplication.
- Some data prepartion was involved in order to make column values more concise/readable using excel's find and replace feature. 
- No power query or data modelling aspects were used. These features will be used later in Power BI projects.
- The inital dataset contained approximatley 104k rows and 25 columns. Worked dataset has the same number of rows but 32 columns now.
- Passenger IDs were changed from 1 to 

## Dashboard Sections

 1. Service Ratings by Passenger Experience Area

This section compares the average rating across different passenger experience areas.

The lowest-rated areas which fell below the overall service score were highlighted to identify where Centauri Airlines may need to focus improvement efforts.

 2. Dynamic Top and Bottom 5 Experience Areas by Flight Class

A data validation dropdown allows the user to select a flight class: Business, Economy, or Economy Plus.

The dashboard then dynamically shows the top 5 and bottom 5 passenger experience areas for the selected class.

3. Age Group Profile

This section shows passenger count and Overall Service Score by age group.

It helps identify which age groups make up the largest share of the passenger base and how the overall service score varies by different age groups.

4. Overall Passenger Satisfaction

A donut chart shows the overall split between satisfied and neutral/dissatisfied passengers.

This gives a high-level view of customer satisfaction.

5. Overall Service Score vs Satisfaction Rate

This section analyses how satisfaction rate changes across Overall Service Score bands.

It shows whether passengers with higher service scores are more likely to be satisfied.

6. Flight Class vs Satisfaction

A 100% stacked bar chart shows satisfaction split by flight haul.

It shows that satisfaction can vary greatly by flight class. 

7. Customer Loyalty vs Satisfaction

A 100% stacked bar chart compares satisfaction between loyal and non-loyal passengers.

This helps assess whether the airline’s core passenger base is satisfied.

---

## Key Insights

- Inflight service and baggage handling were consistent strengths across all flight classes, while inflight Wi-Fi and ease of online booking were recurring weaknesses, highlighting digital experience as a key improvement area.
- Overall passenger satisfaction was below 50%, showing clear room for improvement.
- Higher Overall Service Score was strongly associated with higher satisfaction rate.
- Centauri Airlines’ average Overall Service Score was approximately 3.28, placing it in the 3.00-3.49 OSS band.
- Passenger volume was concentrated mainly in the 25–54 age range. There's no significant variation as to how different age groups rate us.
- Higher satisfaction on longer-haul flights appears largely driven by a greater concentration of Business Class passengers, who reported higher service ratings and therefore were more likely to be satisfied.
- Loyal passengers had a higher satisfaction rate than non-loyal passengers, but satisfaction among loyal passengers was still below 50%.

---

## Recommendations

Based on the analysis, Centauri Airlines should prioritise improving weaker controllable service areas such as inflight Wi-Fi and ease of online booking.
Improving these areas could help increase the Overall Service Score and move more passengers into higher satisfaction bands.
The airline should also focus on its loyal passenger base, as loyal passengers represent a large share of the dataset but still show significant room for satisfaction improvement.

---

## Files Included

- `Centauri_Airlines_Passenger_Satisfaction_Dashboard.xlsx`  
  Excel workbook containing the dashboard, analysis, working data, and supporting calculations.

- `dashboard-preview.png`  
  Dashboard preview image.

---

## Project Status
Completed first version of the Excel dashboard. Further refinements may include additional documentation, deeper insight summaries, and portfolio write-up improvements.
