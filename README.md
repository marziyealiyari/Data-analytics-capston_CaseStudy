# Bellabeat Case Study Analysis

Welcome to the Bellabeat Smart Device Usage Analysis project! This repository contains data exploration, cleaning, and analysis performed on smart device usage (Fitbit data) to uncover behavioral trends and generate marketing insights for Bellabeat, a health-focused tech company specializing in wellness products for women.

---

## 📘 About Bellabeat

**Founded** in 2014, **Bellabeat** designs smart wellness technology tailored specifically for women. Their product ecosystem empowers users to track and optimize various aspects of their well-being — including physical activity, sleep, stress, hydration, and mindfulness.

### 🌟 Key People
- **Urška Sršen**: Co-founder and Chief Creative Officer  
- **Sando Mur**: Co-founder and Executive Team Member  

### 🛍️ Product Line
- **Bellabeat App**: Tracks activity, sleep, menstrual cycle, mindfulness, and more.
- **Leaf**: A wellness tracker wearable (bracelet, necklace, or clip).
- **Time**: A smart wellness watch.
- **Spring**: A smart water bottle that tracks hydration.
- **Bellabeat Membership**: Personalized insights on health, fitness, sleep, and mindfulness.

---

## 📌 Case Study Overview

As a junior data analyst on Bellabeat’s marketing analytics team, your task was to explore how consumers use non-Bellabeat smart devices (Fitbit data) to uncover trends and insights that could inform marketing strategies for Bellabeat products.

### 🎯 Business Objective

- Identify trends in smart device usage
- Determine how these trends relate to Bellabeat customers
- Provide actionable recommendations for marketing strategy

---

## 📂 Data Sources

**Fitbit Fitness Tracker Dataset**  
Collected from 30 users over 31 days.  
Analyzed files:
- `dailyActivity_merged.csv`
- `sleepDay_merged.csv`

---

## 🛠️ Tools & Libraries

- R
- tidyverse
- ggplot2
- dplyr
- janitor
- lubridate
- skimr
- tidyr

---

## 🔄 Data Cleaning & Preparation

- Standardized and reformatted date fields (`mdy`, `mdy_hms`)
- Removed empty and null-filled columns
- Verified user ID consistency across datasets
- Checked for duplicates and joined `activity` and `sleep` data by `id` and `date`

---

## 📊 Analysis Summary

### 🔹 A. Activity Trends

- **Average Steps**: Most users didn’t meet the recommended 10,000 daily steps
- **Sedentary Time**: High across all users; physical inactivity is common
- **Active Minutes**: Very low for most, especially Very Active Minutes

### 🔹 B. Sleep Patterns

- **Inconsistent Sleep**: Most users had irregular sleep schedules
- **Average Sleep Duration**: 6–7.5 hours/night
- **Strong Correlation**: More time in bed correlates with more time asleep

### 🔹 C. Engagement

- **Logging Frequency**: Some users tracked daily; others only a few days
- **Sleep Tracking**: Less consistent than activity logging
- **Engagement Variance**: Users showed wide-ranging commitment

### 🔹 D. Sleep & Activity Correlation

- **Positive Relationship**: Users who sleep more tend to be more active

---

## 📈 Visualizations

- Scatterplot: Sleep vs. Bedtime, Activity vs. Sedentary Minutes
- Histogram: Distribution of Sleep Duration
- Correlation Plots: Step Count vs. Sleep Duration
- Summary Tables: Steps per user, average sleep, device usage

---

## 💡 Key Findings

| Insight | Observation |
|--------|-------------|
| **Low Physical Activity** | Most users fall short of 10,000 steps/day |
| **High Sedentary Time** | Users spend the majority of the day inactive |
| **Inconsistent Sleep** | Varying sleep duration & timing |
| **Inconsistent Engagement** | Wide range in tracking frequency |
| **Positive Sleep-Activity Link** | Users who sleep more are more active |

---

## 📌 Product Focus: Bellabeat Leaf or Time

Both devices track **activity**, **sleep**, and **stress**, making them suitable for applying these behavioral insights.

---

## 📣 Marketing Strategy Recommendations

### ✅ Promote Daily Micro-Habits
Use app notifications to encourage short activities (e.g., 10-minute walks).

### 🔁 Boost Weekly Engagement
Send weekly check-ins:  
*"You’ve tracked 3/7 days – try for 5 next week!"*

### 🌙 Connect Sleep & Movement
Emphasize how better sleep can lead to better activity — “Sleep better, move more!”

### ⏰ Timely Notifications
Push notifications during evening downtime (5–8 PM) for higher impact.

### 🎯 Gamified Progress
Visualize streaks for sleep, hydration, and steps to boost motivation.

### 📚 Educate via Membership
Create rich content explaining the connection between sleep, stress, and wellness.

---

## 📅 Timeline

This case study was completed within **one week** as a guided data analysis exercise.

---

## 📁 Repository Structure

```bash
├── README.md
├── Bellabeat_Case_Study.Rmd / .ipynb
├── /data
│   ├── dailyActivity_merged.csv
│   └── sleepDay_merged.csv
├── /visuals
│   ├── sleep_histogram.png
│   └── engagement_scatter.png
