# Marketing Analysis

## Project Overview

This project conducts a thorough analysis of a marketing A/B test dataset, evaluating the effectiveness of two different advertising strategies: traditional ads (`ad`) and public service announcements or no ads (`psa`). The analysis encompasses data exploration, visualization, cross-tabulation, and statistical testing to derive insights about the impact of each strategy on user conversion rates.

# About Dataset

## Marketing A/B testing dataset

Marketing companies want to run successful campaigns, but the market is complex and several options can work. So normally they tun A/B tests, that is a randomized experimentation process wherein two or more versions of a variable (web page, page element, banner, etc.) are shown to different segments of people at the same time to determine which version leaves the maximum impact and drive business metrics.

The companies are interested in answering two questions:

* Would the campaign be successful?
* If the campaign was successful, how much of that success could be attributed to the ads?

With the second question in mind, we normally do an A/B test. The majority of the people will be exposed to ads (the experimental group). And a small portion of people (the control group) would instead see a Public Service Announcement (PSA) (or nothing) in the exact size and place the ad would normally be.

The idea of the dataset is to analyze the groups, find if the ads were successful, how much the company can make from the ads, and if the difference between the groups is statistically significant.

### Data dictionary:

* Index: Row index
* user id: User ID (unique)
* test group: If "ad" the person saw the advertisement, if "psa" they only saw the public service announcement
* converted: If a person bought the product then True, else is False
* total ads: Amount of ads seen by person
* most ads day: Day that the person saw the biggest amount of ads
* most ads hour: Hour of day that the person saw the biggest amount of ads

### Objectives

- **Assess the impact** of `ad` and `psa` on user conversion rates.
- **Identify user behavior patterns** based on different advertising strategies.
- **Evaluate the statistical significance** of differences observed between the `ad` and `psa` groups.

## Project Structure

### 1. Data Exploration
- **Initial Data Cleaning:** Removed unnecessary columns and inspected the dataset for missing values.
- **Unique User IDs:** Ensured the uniqueness of user IDs to maintain data integrity.

### 2. Data Visualization
- **Group Distribution:** Visualized the distribution of users in the `ad` and `psa` groups.
  
![image](https://github.com/user-attachments/assets/d05f86c3-c219-4262-be1d-428694f28646)

- **Conversion Status:** Analyzed and visualized conversion status across the dataset.
  
![image](https://github.com/user-attachments/assets/ba290faa-ebb2-4408-9d53-7c385ff9adf7)

- **Ad Activity Analysis:**
  - **By Day of the Week:** Examined advertisement activity by day of the week.

    ![image](https://github.com/user-attachments/assets/cab19fb0-3368-4c16-bd14-401ee1c75058)

  - **By Hour of the Day:** Analyzed ad activity based on the hour of the day.

    ![image](https://github.com/user-attachments/assets/67e77d17-a568-42a2-9152-bae5faf7452e)

  - **Ad Views Distribution:** Explored the distribution of the number of ads seen by users.
 
    ![image](https://github.com/user-attachments/assets/76a38ec5-33eb-4767-a597-adcd05700417)



### 3. Cross-Tabulation Analysis
- **Test Group vs. Conversion:**
  - Created a crosstab to analyze conversion rates within the `ad` and `psa` groups.
  - Employed styling to highlight significant differences.

  ![Conversion Crosstab]![image](https://github.com/user-attachments/assets/08330228-2b54-496e-8637-1034a75507c3)


- **Conversion Rates by Day of the Week:**
  - Created and styled crosstabs to compare conversion rates across different days of the week for the `ad` group.
  - Applied the Chi-Square test to assess the independence of conversion rates and specific days.

  ![Day Conversion Crosstab]![image](https://github.com/user-attachments/assets/60e73969-fadd-4b6d-986e-8a865e3b3fde)


- **Conversion Rates by Hour of the Day:**
  - Analyzed conversion rates across different hours of the day using crosstabulations.
  - Sorted and styled the results to identify peak hours for ad effectiveness.

  ![Hour Conversion Crosstab]![image](https://github.com/user-attachments/assets/c9ed3bbb-e6a5-4486-a891-6402484587a0)


### 4. Statistical Testing
- **Z-Test for Conversion Rates:**
  - **Objective:** Conducted a two-proportion Z-test to determine if the difference in conversion rates between the `ad` and `psa` groups is statistically significant.
  - **Result:** Identified a significant difference, suggesting that the `ad` group outperforms the `psa` group in conversion rates.

  ![Z-Test Results]![image](https://github.com/user-attachments/assets/6b205185-0aa6-4d30-bfbe-d32e0a8cb739)


- **Chi-Square Test for Independence:**
  - **Objective:** Tested the independence of conversion rates with respect to the day of the week and hour of the day within the `ad` group.
  - **Result:** Certain days and hours were found to have a significant impact on conversion rates.
    
    ![image](https://github.com/user-attachments/assets/96253cc7-ad73-4a7c-80e3-83f1bbe3d8fc)

    ![image](https://github.com/user-attachments/assets/770e4220-2609-4586-81e6-eee7b7d008e1)


- **Effect Size Calculation (Cohen's d):**
  - **Objective:** Calculated Cohen's d to measure the magnitude of the difference in conversion rates between the `ad` and `psa` groups.
  - **Result:** Provided a quantitative measure of the effect size, indicating how much the `ad` strategy influences conversion rates.

  ![Effect Size]![image](https://github.com/user-attachments/assets/f5bd233c-386a-4a0c-9c73-32f870bff2ec)


### 5. Detailed Analysis
- **Crosstabs and P-Value Matrices:**
  - **Objective:** Generated detailed crosstabs and p-value matrices to explore relationships between conversion rates and specific days within the `ad` group.
  - **Focus Areas:** Emphasized weekdays vs. weekends, with a special focus on particular days like Monday and Tuesday.

  ![P-Value Matrix]![image](https://github.com/user-attachments/assets/99b234e3-a8ad-4f19-92bf-39337667573a)


- **Hourly Ad Analysis:**
  - **Objective:** Evaluated the effectiveness of ad displays by hour of the day using crosstabs and statistical testing.
  - **Key Findings:** Identified peak hours that maximize conversion rates, providing insights for optimizing ad schedules.

  ![Hourly Ad Analysis]![image](https://github.com/user-attachments/assets/c8d5682a-69cc-4491-9b68-c86b4c32fa89)


## Conclusion
The analysis provides actionable insights into the effectiveness of traditional ads compared to public service announcements. Key findings suggest that optimizing ad exposure by time of day and specific days of the week could significantly enhance conversion rates.
