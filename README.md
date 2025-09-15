Project (overview)
- Global Overview — KPI cards, world map, top-10 countries bar chart
- Charging Infrastructure — power class donut, station density map, power distribution
- EV Models Analysis — make/model matrix, market treemap, timeline
- Country Comparison — country metrics matrix and small multiples
Key measures (examples in report)
- Total Stations = COUNT(charging_stations_2025_world[id])
- Average Power = AVERAGE(charging_stations_2025_world[power_kw])
- Fast DC % = DIVIDE(COUNTROWS(FILTER(charging_stations_2025_world, charging_stations_2025_world[is_fast_dc] = TRUE)), COUNTROWS(charging_stations_2025_world))
- Total Ports = SUM(charging_stations_2025_world[ports])
- Avg Ports per Station = DIVIDE([Total Ports], [Total Stations])
🛠️ Tools & Technologies

* **Data Visualization:** Power BI Desktop
* **Data Transformation:** Power Query (M Language)
* **Data Modeling & Calculations:** DAX
* Data Sources
- CSV files
