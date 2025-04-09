# BigData-Trucking-Risk-Analysis

### 🎯 Problem Statement

As the fleet manager of **Arizona National Trucking (ANT)**, our foremost challenge is to ensure adherence to company regulations, aiming to reduce insurance risks. This encompasses tackling issues such as **speeding**, **unsafe following distances**, **lane departure incidents**, and other hazardous driving practices among our fleet drivers.

### 🎯 Objectives

- Assist fleet managers in identifying dangerous drivers with a **risk threshold greater than 7**
- Identify **hazardous truck models** used across the country
- Detect **violations based on geographic location**
- Analyze how much **drivers, truck models, and locations** contribute to overall risk

---
### How This Project Was Done

This Big Data Analytics project focuses on assessing trucking risks using event-based driver data. The entire process included:

1. **Problem Understanding:** We began by identifying real-world challenges in fleet management related to driver safety and insurance risks.

2. **Data Collection & Preprocessing:** Raw driver data, vehicle records, and event logs were cleaned and formatted for analysis. This step included:
   - Removing duplicates
   - Filtering out incomplete or irrelevant entries
   - Normalizing values such as speed and distance

3. **Data Storage in Hive:** Cleaned data was imported into **Hive** where we:
   - Created structured **tables** for drivers, trucks, events, and risk metrics
   - Used **HiveQL** queries to aggregate data and calculate metrics like risk factors per driver, truck model, and region

4. **Data Modeling:** Risk scores were generated based on factors such as:
   - Event frequency
   - Distance driven
   - Type of violations (e.g., lane departure, speeding, unsafe following)
   - Geographic location of incidents

5. **Visualization with Tableau:** Data from Hive tables was exported and visualized using **Tableau**. We created:
   - Dashboards showing high-risk drivers and trucks
   - Heatmaps of high-risk zones across the country
   - Bar and pie charts for event distribution

6. **High-Risk Identification:** 
   - Flagged drivers with risk scores above 7
   - Highlighted truck models contributing to frequent violations
   - Mapped geographic zones with the highest risk

7. **Insights & Recommendations:** 
   - Driver **A97** recommended for license suspension
   - High-risk models like **Ford**, **Peterbilt**, and **Caterpillar** identified
   - Recommendations included installing lane-assist systems and creating driver incentives

This project used **Apache Hive** for scalable data storage and querying, and **Tableau** for interactive dashboards, providing clear and actionable insights to reduce risk in the trucking industry.

