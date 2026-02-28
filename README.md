# Bank-Fraud-Analysis-Power-Bi
## Table of Contents
- [Description](description)
- [Business Problems](businessproblems)
- [Dashboards](dashboards)
- [Key Analytical Findings](keyanalyticalfindings)
- [Recommendations](recommendations)
- [Limitations](limitations)
  
### Description
This Power BI dashboard was developed to analyze digital banking transactions and identify fraud patterns, transaction behavior, and network performance impact.
The solution provides interactive analysis across three main areas:
- Executive Overview
- Fraud Detection
- Transaction Level Details
  
### Business Problems
#### Financial institutions need to:
- Monitor transaction volumes and financial exposure
- Detect fraud trends early
- Identify high-risk transaction types and devices
- Understand whether network Slice affects transaction outcomes
#### This dashboards answers:
1.	What is the overall transaction volume and value?
2.	Is fraud increasing over time?
3.	Which transaction types have the highest fraud rate?
4.	Which devices are most associated with fraudulent transactions?
5.	Are certain regions or network slices riskier?

## Dashboards
### Home Page (Executive Summary)
#### Key Insights 
-	Total Transactions: 1000
-	Total Transaction Value: £771,170
-	Success Rate: 48.7%
-	Failed Transactions: 51.3%
-	Most common transaction type: Transfer
-	Highest transaction region: Europe
  
<img width="1438" height="807" alt="Screenshot 2026-02-28 145148" src="https://github.com/user-attachments/assets/fb8ccf4c-0826-4d27-a6f5-55d13477286d" />

### Fraud Detection Page
#### Key Insights
#### Which transaction type has the highest fraud exposure?
- Transfer accounts for the highest proportion of fraudulent transactions of approx. 35%.
#### Which device is most associated with fraud?
- Mobile devices show the highest fraudulent transaction value of approx. 208.66k suggesting increased behavioral risk.
#### Is fraud increasing over time?
- Fraud transactions show a downward trend between 10:30AM and 11:00AM, peaking at approximately 10:55AM.
#### Are certain network slices more vulnerable?
- Slice 2 recorded the highest number of fraudulent transactions at 173, indicating potential monitoring gaps.

<img width="1441" height="807" alt="Screenshot 2026-02-28 145133" src="https://github.com/user-attachments/assets/9af434d9-fcb9-46e1-8a08-3aa2ca82a7e8" />

### Transaction Details
#### Key Purpose
- Drill-through capability for fraud investigation
-	Validate fraud clusters seen in summary visuals

<img width="1443" height="805" alt="Screenshot 2026-02-28 145220" src="https://github.com/user-attachments/assets/15e2ed36-3d4b-4a4d-9c32-e19437a2eaee" />

### DAX Measures Created
-	Total Transactions
-	Total Transaction Amount

### Interactive Features
#### The following Slicers were implemented for dymanic interaction accross all pages:
-	Transaction Type
-	Device Used
-	Transaction Status
-	Fraud Flag

## Key Analytical Findings
#### Fraud Exposure Is Financially Significant
- Fraudulent transactions represent a measurable portion of total transaction volume and transaction value, indicating meaningful financial risk exposure. Even where fraud volume appears moderate, the associated transaction amounts suggest concentrated high value fraud cases.
#### Fraud Concentration by Transaction Type
- Transfers account for a higher proportion of fraudulent transaction value compared to others. This indicates that fraud risk is not evenly distributed and is likely linked to transaction characteristics rather than overall volume alone.
#### Device Based Risk Patterns
-Fraudulent transactions are more concentrated on Mobile devices, suggesting behavioral vulnerabilities on certain platforms.
#### Time-Based Fraud Spikes
- Fraudulent transaction trends show identifiable peaks during specific time intervals, indicating potential opportunistic fraud behavior during high volume or lower monitoring periods.
#### Network Slice Variation
-Transaction distribution across network slices is uneven, and some slices show relatively higher fraud counts. While not necessarily causal, this may suggest performance or monitoring gaps within specific network segments.

## Recommendations
1.	Implement stricter authentication for high risk transaction types.
2.	Increase monitoring on devices with higher fraud association.
3.	Conduct further investigation into network slices with higher fraud  to determine whether performance degradation contributes to abnormal transaction behavior.
4.	Implement real time alert thresholds during peak fraud hours identified in the analysis.

## Limitations
1.	The dataset represents simulated environment and may not reflect real world behavioral complexity.
2.	The analysis does not include historical customer transaction patterns, which limits behavioral anomaly detection.
3.	Fraud insights rely on the accuracy of the existing Fraud Flag variable. If fraud labelling is incomplete or delayed, insights may underestimate actual fraud exposure.

#### This project demonstrates the application of descriptive analytics, KPI modelling, and fraud pattern analysis using Power BI. The dashboard enables both operational monitoring and strategic risk assessment through interactive exploration and targeted insights.









