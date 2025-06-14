Created this PowerBI Dashboard of Air Pollution Data with self build dataset 
 
📊 🚀 Building a Pollution Dashboard in Power BI
👉 Key Insights:

📊 Most Polluted State: Uttar Pradesh with an Avg AQI of 350.
🌿 Least Polluted State: Kerala with an Avg AQI of 42.
🟥 Highest AQI: North India (Avg AQI: 280)
🟩 Lowest AQI: South India (Avg AQI: 75)
⚠️ 25% of the cities are in the Hazardous category—posing serious health risks
📈 Peak Pollution: December (Avg AQI: 320) – Possibly due to winter smog.
📉 Cleanest Month: July (Avg AQI: 90) – Likely due to monsoon rains.
🏙️ Top 5 Polluted Cities:
Delhi – Avg AQI: 345
Ghaziabad – Avg AQI: 330
Noida – Avg AQI: 325
Lucknow – Avg AQI: 310
Patna – Avg AQI: 295
🤌 Kerala and Sikkim maintain consistently clean air year-round.
✅ Step 1: Data Cleaning in Power Query
I started by cleaning the dataset—removing duplicates, handling missing values, and ensuring data accuracy for better analysis.
✅ Step 2: Create ‘Month-Year’ Column
To track pollution trends over time, I extracted the Month-Year from the date column.
👉 DAX Formula:
Month-Year = FORMAT('Table'[Date], "MMM-YYYY")
✅ Step 3: Create a Date Slicer
I added a date slicer to allow users to dynamically filter and explore pollution data by time range.
✅ Step 4: Add a Region Pollution by State Pie Chart
I used a pie chart to show pollution distribution across Indian regions, helping visualize state-wise contributions to pollution.
✅ Step 5: Create 'Region_Pollution' Measure
I calculated total pollution by region using the SUM function for accurate aggregation.

✅ Step 6: Add a Region Slicer
I added an interactive slicer to filter data by regions, making the dashboard more user-friendly.
✅ Step 7: Create an AQI Category Column
I classified AQI levels into categories like Good, Moderate, and Hazardous for better interpretation.
✅ Step 8: Apply Dynamic Conditional Formatting
I used conditional formatting on the Avg_AQI card to highlight pollution levels visually:
🟢 Green for Good
🟡 Yellow for Moderate
🔴 Red for Hazardous
✅ Step 9: Create Relationships Between Tables
I established one-to-many relationships between tables (City, State, and Region) for better data modeling and cross-filtering.
✅ Step 10: Add a Dynamic Tooltip
I added a custom tooltip to provide detailed information (State, Region, AQI) when hovering over the pie chart—enhancing data storytelling.
