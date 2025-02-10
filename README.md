# WAZE
WAZE PROJECT
**User Churn Project - Executive Summary**

**Prepared for:** Waze Leadership Team  

![image](https://github.com/user-attachments/assets/b3bafd1e-ecba-4713-aa71-a89c69200892)


### **Project Overview**
The Waze data team is conducting an analysis to prevent monthly user churn by identifying behavioral patterns associated with app uninstallation or inactivity. The dataset includes information on user engagement, driving behaviors, and device types, allowing us to compare churned versus retained users and develop strategies to enhance retention.

### **Key Findings**
- **User Churn Distribution:** The dataset contains **82% retained users** and **18% churned users**.
- **Missing Data:** The `label` column contains **700 missing values**, but the missing data appears to be random.
- **Driving Patterns:**
  - Churned users averaged **~3 more drives per month** than retained users.
  - Retained users used the app on **twice as many days** as churned users.
  - The median churned user drove **~200 km more per month** and spent **2.5 more hours** on the road compared to retained users.
  - Churned users took **fewer but longer** trips, averaging **698 km per driving day**, which is **240% more distance per day than retained users**.
- **Device Analysis:**
  - No significant difference in churn rates between **iPhone and Android users**.
  - Both device types showed similar retention trends, suggesting that device experience is not a primary driver of churn.
- **New Feature Engineering:**
  - **km_per_drive**: Distance driven per trip.
  - **km_per_driving_day**: Distance driven per active day.
  - **drives_per_driving_day**: Number of trips taken per active day.

### **Recommendations & Next Steps**
1. **Target High-Usage Drivers:**
   - Churned users tend to take **longer and more frequent trips in a shorter time frame**.
   - Further investigate whether high-usage drivers face app usability issues.
2. **Enhanced Personalization:**
   - Implement user-specific engagement strategies, such as custom notifications or in-app incentives.
3. **Gather Additional Data on Super-Drivers:**
   - These users may have **unique needs** (e.g., truck drivers, couriers). Waze could introduce **tailored features** to enhance their experience.
4. **Develop Predictive Model for Churn Risk:**
   - Use machine learning to classify at-risk users and deploy retention strategies before they churn.
5. **Data Visualization & Further EDA:**
   - Conduct **in-depth exploratory data analysis (EDA)** and develop data visualizations to illustrate key insights.

### **Conclusion**
The analysis suggests that churned users drive more frequently but use the app on fewer days. Waze can leverage this insight to **enhance retention efforts through targeted engagement and feature improvements**. The next phase involves developing a **predictive churn model** and conducting deeper EDA to refine our understanding of churn behaviors.

