# Marketing A/B Test Analysis
Project Overview
This project conducts a thorough analysis of a marketing A/B test dataset, evaluating the effectiveness of two different advertising strategies: traditional ads (ad) and public service announcements or no ads (psa). The analysis encompasses data exploration, visualization, cross-tabulation, and statistical testing to derive insights about the impact of each strategy on user conversion rates.

Objectives
Assess the impact of ad and psa on user conversion rates.
Identify user behavior patterns based on different advertising strategies and times of the day.
Evaluate the statistical significance of differences observed between the ad and psa groups.
Project Structure
1. Data Exploration
Initial Data Cleaning: Removed unnecessary columns and inspected the dataset for missing values.
Unique User IDs: Ensured the uniqueness of user IDs to maintain data integrity.
2. Data Visualization
Group Distribution: Visualized the distribution of users in the ad and psa groups.

Conversion Status: Analyzed and visualized conversion status across the dataset.

Ad Activity Analysis:

By Day of the Week: Examined advertisement activity by day of the week.
By Hour of the Day: Analyzed ad activity based on the hour of the day.
Ad Views Distribution: Explored the distribution of the number of ads seen by users.
Image Suggestion: Include visualizations such as bar charts or histograms to illustrate the distribution of users in each group, conversion rates, and ad activity patterns.

3. Cross-Tabulation Analysis
Test Group vs. Conversion:

Created a crosstab to analyze conversion rates within the ad and psa groups.
Employed styling to highlight significant differences.
Image Suggestion: Display the crosstab with color-coded cells to emphasize the conversion rates for the ad and psa groups.

Conversion Rates by Day of the Week:

Created and styled crosstabs to compare conversion rates across different days of the week for the ad group.
Applied the Chi-Square test to assess the independence of conversion rates and specific days.
Image Suggestion: Include a heatmap or matrix plot of the Chi-Square test results to visualize significant p-values across different days.

Conversion Rates by Hour of the Day:

Analyzed conversion rates across different hours of the day using crosstabulations.
Sorted and styled the results to identify peak hours for ad effectiveness.
Image Suggestion: Use a time-based plot or bar chart to showcase the conversion rates by hour of the day.

4. Statistical Testing
Z-Test for Conversion Rates:

Objective: Conducted a two-proportion Z-test to determine if the difference in conversion rates between the ad and psa groups is statistically significant.
Result: Identified a significant difference, suggesting that the ad group outperforms the psa group in conversion rates.
Image Suggestion: Include a bar plot comparing conversion rates between the two groups with Z-test results highlighted.

Chi-Square Test for Independence:

Objective: Tested the independence of conversion rates with respect to the day of the week and hour of the day within the ad group.
Result: Certain days and hours were found to have a significant impact on conversion rates.
Effect Size Calculation (Cohen's d):

Objective: Calculated Cohen's d to measure the magnitude of the difference in conversion rates between the ad and psa groups.
Result: Provided a quantitative measure of the effect size, indicating how much the ad strategy influences conversion rates.
Image Suggestion: Visualize the effect size results with a bar chart comparing Cohen's d values for different segments.

5. Detailed Analysis
Crosstabs and P-Value Matrices:

Objective: Generated detailed crosstabs and p-value matrices to explore relationships between conversion rates and specific days within the ad group.
Focus Areas: Emphasized weekdays vs. weekends, with a special focus on particular days like Monday and Tuesday.
Image Suggestion: Display these crosstabs with highlighted cells for significant differences.

Hourly Ad Analysis:

Objective: Evaluated the effectiveness of ad displays by hour of the day using crosstabs and statistical testing.
Key Findings: Identified peak hours that maximize conversion rates, providing insights for optimizing ad schedules.
Image Suggestion: Include line charts or heatmaps showing conversion rates across different hours of the day.

Conclusion
The analysis provides actionable insights into the effectiveness of traditional ads compared to public service announcements. Key findings suggest that optimizing ad exposure by time of day and specific days of the week could significantly enhance conversion rates.
