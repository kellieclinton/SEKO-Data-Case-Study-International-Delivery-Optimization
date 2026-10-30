# Python Projects Portfolio

Welcome to my Python portfolio! This repository contains data science, engineering, and business analytics projects focused on solving real-world operational problems.

---

## 🚚 From 50% to 90%: Optimizing International Delivery Success
A comprehensive data analytics case study evaluating the operational lifecycle of approximately 8,000 international shipments. The purpose of this analysis was to determine why package deliveries fall behind schedule and how to systematically bridge the gap to achieve a 90% on-time delivery rate.

*Note: This project was originally completed as a take-home technical assessment during an interview loop. The internal team highly praised the depth of analysis, code structure, and actionable business insights.*

### 📌 Project Objectives
1. **Identify Systemic Bottlenecks:** Determine if delivery delays are localized to specific carriers/lanes or systemic across the logistics network.
2. **Isolate Drivers of Lateness:** Evaluate operational factors, handoff limits, and estimation accuracy.
3. **Formulate Data-Driven Solutions:** Provide clear algorithmic and operational boundaries to scale performance to a 90% success baseline.

### 🛠️ Data Engineering & Cleansing
* **Normalization:** Used Excel to cleanse, format, and normalize disparate estimated and actual delivery timestamps into a single, cohesive timezone (UTC).
* **Reliability Filtering:** Isolated and validated active delivery cycles using verified status tracking. Non-delivered cycles (Exceptions, Holds, In-Transit) were structurally segmented for secondary investigation due to the unstructured, multilingual nature of the exception records.

### 📈 Key Insights & Strategic Recommendations
* **The Over-Promising Problem:** Analysis revealed that packages were exactly 50% likely to be late. Delays were not driven by individual carriers or specific lanes, but rather by a systemic underestimation algorithm lacking a realistic logistics "padding."
* **The 90% Confidence Solution:** Proposed adding an 18 to 19-hour buffer to estimated delivery windows globally to drop the late delivery rate from 50% down to 10%.
* **The Sunday Paradox:** Discovered that while Sunday deliveries have the lowest overall failure frequency, they suffer from the highest failure severity (19.1-hour average delays) when a breakdown occurs.
* **The 20-Handoff Operational Cap:** Identified that logistics streams remain stable up to 5 handoffs, but experience extreme volatility and catastrophic failure rates past 20 touches. Recommended a strict operational limit of 20 handoffs maximum to preserve the baseline.
