# Sports Injuries Analytics & Performance Insights: A Data-Driven Approach to Athlete Health Management

## 📖 About this Project

In modern competitive sports, player availability and health management are critical to achieving consistent performance and long-term success. Sports organizations face the dual challenge of keeping athletes in peak condition while minimizing injury-related downtime and controlling treatment costs. To meet these demands, medical teams, coaches, and performance analysts require real-time, data-driven insights into injury patterns, treatment effectiveness, and workload management.

The Sports Injuries Analytics & Performance Insights dashboard is a comprehensive Power BI solution designed to track and analyze injuries, recovery times, treatment outcomes, and related costs. It enables decision-makers at all levels—team doctors, physiotherapists, coaches, performance analysts, and senior management—to quickly identify high-risk players, evaluate treatment efficiency, and optimize training programs to reduce injury recurrence. By integrating diverse datasets into a centralized star schema data model and leveraging advanced DAX measures, the solution offers a consolidated, interactive view of core sports health KPIs, including total injuries, average recovery time, treatment costs, player workload before injury, and top injury types.

The rationale behind this solution stems from a common issue in sports management: injury and treatment data is often fragmented across different systems—medical records, training logs, match statistics, and cost reports—making it difficult to obtain a clear and timely overview. This fragmentation hinders proactive injury prevention and delays corrective action. This dashboard bridges the gap by providing a single source of truth for player health and performance-related injury data.

At the core of the solution lies a single fact table—FactInjuries—which consolidates injury events, treatment details, and recovery metrics. This is enriched by multiple dimension tables (DimPlayer, DimInjuryType, DimClub, DimEvent, DimTreatment, DimCoach, DimLocation, and Calendar) to enable granular slicing and filtering by player, injury type, club, event, treatment method, coach, and location. Data modeling practices included building surrogate keys, cleaning categorical fields, creating calculated columns such as Days to Recovery and Treatment Cost per Minute Played, and implementing time intelligence using the Calendar table.

<img width="1552" height="820" alt="Modelling_Sport Injury" src="https://github.com/user-attachments/assets/e2e326e2-012b-407f-b60f-754ff46200b1" />

---

## 📄 Page 1 – Injury Overview & Trends

The first page of the dashboard delivers an executive-level view of injury frequency, recovery patterns, and treatment costs over time. It is designed to help medical staff, coaching teams, and management quickly identify which injury types occur most frequently, when injury peaks occur, and the overall cost burden on the organization. At the top of the page, four prominent KPIs present an at-a-glance summary: Total Injuries (15K), Average Absence (48.71 days), Total Treatment Cost (£27.70M), and Top Injury Type (Fracture). These figures establish a performance baseline and highlight areas requiring immediate attention.

Supporting visuals provide deeper context. Bar charts compare injury occurrences by quarter and season, making it easy to spot high-risk periods in the sporting calendar. A treemap ranks injury types by frequency, with fractures, tendon injuries, and concussions emerging as the most common, helping medical teams target prevention programs toward the most impactful injury categories. A line chart tracks treatment cost fluctuations over time, revealing cost spikes that may align with high injury periods or expensive treatments. Finally, a matrix table offers a side-by-side comparison of injury types, showing total injuries, average recovery time, and total treatment cost. This combination of visuals and KPIs provides decision-makers with the information needed to allocate resources, control costs, and proactively manage player health.

<img width="1442" height="799" alt="Page 1" src="https://github.com/user-attachments/assets/87d40727-54bf-48e8-8345-365c0104e970" />

---

## 📄 Page 2 – Player & Treatment Insights

The second page focuses on a detailed analysis of individual players, treatment efficiency, and recovery outcomes. It answers crucial questions such as: Which players are sustaining the most injuries? Which treatments are most commonly applied? How does workload impact recovery time? The top KPIs displayed are Average Treatment Cost (£1.85K), Treatment Count (18), Total Treatment Cost (£27.70M), and Top Injury Type (Fracture). These provide a concise summary of the treatment landscape and cost structure.

The page begins with bar charts showing the injury types that required the highest number of treatments, alongside a ranking of players with the most recorded injuries. This instantly identifies high-risk players and injury types that demand more resources. A scatter plot compares minutes played in the last 30 days against recovery time, uncovering potential workload-related injury patterns. If a player has a high workload and a long recovery time, this may indicate the need for load management or rest periods. A donut chart segments treatment outcomes into categories such as Fully Recovered, Recovered with Issues, and Retired, providing insight into the effectiveness of treatments. A matrix table organizes players by their total treatment costs, broken down by injury severity (Minor, Moderate, Severe). This helps in understanding cost drivers at the player level and can inform decisions on treatment strategies, medical budget allocation, and contract negotiations.
<img width="1448" height="820" alt="Page 2" src="https://github.com/user-attachments/assets/ca03facc-7dfa-48d2-bd27-75882c52acaa" />

---

## 📄 Page 3 – Coach & Location Analysis

The third page provides a comprehensive analysis of coaching influence on injuries and the geographic distribution of injury cases. It equips decision-makers with insights into whether certain coaches or locations are associated with higher injury risks. The KPIs here mirror the treatment-focused perspective: Average Treatment Cost (£1.85K), Treatment Count (18), Total Treatment Cost (£27.70M), and Top Country (United Kingdom). These serve as starting points for analyzing injury distribution patterns.

A bar chart compares injuries by severity (Minor, Moderate, Severe), revealing that minor injuries make up the largest proportion of cases, but moderate and severe injuries still represent a significant portion of medical costs and downtime. A map visual plots injury occurrences geographically, identifying high-risk countries and regions. The donut chart shows the gender distribution of coaches, offering demographic context that could be relevant for broader performance and wellness studies. Another bar chart ranks countries by injury count, highlighting where prevention efforts could be concentrated. Finally, a matrix table lists coaches along with average absence days, average treatment costs, and minutes played by their athletes. This allows for direct comparisons and the identification of coaching patterns that may influence injury rates or recovery outcomes.
<img width="1453" height="822" alt="Page 3" src="https://github.com/user-attachments/assets/71f95371-77fd-462d-aad0-395dcfdb1ef3" />

---

## 💡 Key Strategic Insights

Fractures and tendon injuries are the leading causes of long recovery times and high treatment costs, making them prime targets for enhanced prevention programs. High player workload before injury is strongly correlated with longer recovery durations, underscoring the importance of load management. Certain players show consistently high injury frequencies, suggesting overtraining or insufficient recovery protocols. The United Kingdom has the highest injury count, indicating possible environmental, scheduling, or training condition factors. Several coaches oversee players with higher absence rates and treatment costs, pointing to opportunities for refining training methods and medical support.

---

## ✅ Conclusion

The Sports Injuries Analytics & Performance Insights dashboard demonstrates the powerful role of analytics in modern sports health management. By consolidating injury, treatment, and performance data into a unified reporting system, it provides actionable insights for medical teams, coaches, and management alike. Whether used in weekly injury review meetings, seasonal performance evaluations, or long-term health strategy planning, this solution empowers sports organizations to minimize injury risks, improve recovery efficiency, and ensure players are consistently available for selection. With its combination of intuitive design, optimized data modeling, and clear KPIs, the dashboard serves as a vital decision-support tool for achieving both competitive and player welfare goals.
