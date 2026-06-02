UAE Energy Grid Dashboard — Power BI
Overview
An interactive Power BI dashboard analysing energy generation, demand, revenue, emissions and plant efficiency across the UAE — covering Abu Dhabi, Dubai and Sharjah with Solar, Gas and Nuclear power sources.
Built as part of a hands-on Energy Data Analyst portfolio targeting roles in the UAE and India energy sector.

<img width="1171" height="658" alt="BIP1" src="https://github.com/user-attachments/assets/d7eb076b-778c-43f2-b45d-bbd3eebbc77b" />

Dashboard Visuals
VisualPurposeKPI CardsTotal Generation, Demand, Revenue, CO2 Emissions, Avg EfficiencyBar ChartGeneration comparison by EmirateLine ChartMonthly generation trend by energy sourceDonut ChartGeneration mix — Solar vs Gas vs NuclearColumn ChartFuel Cost vs Revenue by PlantTablePlant Efficiency and Downtime Summary

DAX Measures Created
daxTotal Revenue = SUM(UAE_Energy_Dataset[Generation_MWh]) * SUM(UAE_Energy_Dataset[Tariff_AED_per_kWh]) * 1000

Total CO2 = SUM(UAE_Energy_Dataset[CO2_Emissions_Tons])

Avg Efficiency = AVERAGE(UAE_Energy_Dataset[Efficiency_%])

Tools Used

Power BI Desktop
DAX (Data Analysis Expressions)
Power Query
CSV Dataset — 60 rows UAE Energy Data


Dataset Details
AttributeDetailsPower Plants12 plants across UAEEmiratesAbu Dhabi, Dubai, SharjahEnergy SourcesSolar, Gas, NuclearTime PeriodJanuary to May 2023Total Rows60Columns15
Columns included:
Plant_ID, Plant_Name, Emirate, Energy_Source, Month, Generation_MWh, Capacity_MW, Demand_MWh, Fuel_Cost_AED, Maintenance_Cost_AED, CO2_Emissions_Tons, Efficiency_%, Downtime_Hours, Tariff_AED_per_kWh, Revenue_AED

Key Insights from the Dashboard

Abu Dhabi leads total generation — driven by Barakah Nuclear Plant
Nuclear has zero CO2 emissions and the lowest tariff rate (0.18 AED/kWh)
Solar has zero fuel cost — highest revenue margin among all sources
Gas plants carry the highest CO2 footprint and fuel cost burden
Generation mix is currently Gas-dominant — reflecting the UAE's ongoing transition toward Solar and Nuclear under Net Zero 2050


Domain Context
This project reflects the real UAE energy landscape:

DEWA — Dubai Electricity and Water Authority operates Jebel Ali and Mohammed bin Rashid Solar Park
ADNOC / TAQA — Abu Dhabi energy operations including Al Taweelah Gas Plant
Barakah Nuclear Plant — UAE's first nuclear facility, operated by ENEC, contributing zero-carbon baseload power
UAE Net Zero 2050 — national strategy targeting clean energy dominance by 2050

The generation mix donut chart in this dashboard directly visualises the current state of this transition.
