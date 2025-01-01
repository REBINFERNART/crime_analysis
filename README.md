# 📊 Crime Data Analysis Project

## 🚀 Project Overview

This project focuses on analyzing crime trends using a crime dataset. The goal was to preprocess, clean, and analyze the data to uncover insights that could help in understanding and addressing key crime patterns.

---

## 🛠️ Data Preprocessing Steps

### 1️⃣ Handling Duplicates

- **Case Number Column:** Checked for duplicate values and removed any duplicates to ensure data integrity.

### 2️⃣ Dataset Information and Missing Values

- Analyzed dataset information and identified missing values.
- Found missing values in both **discrete** and **continuous** data columns.

### 3️⃣ Filling Missing Values

- **Continuous Columns (Latitude, Longitude, X Coordinate, Y Coordinate, Community Area):**
  - Used `groupby` on the **Block** column.
  - Filled missing values with the **median** of each group (Block-wise analysis showed consistent median values).
  - Remaining missing values were filled with the overall median of the respective columns.
- **Discrete Column (Ward):**
  - Used `groupby` on the **District** column.
  - Filled missing values with the **mode** of each group.

### 4️⃣ Dropping Unnecessary Columns

- Dropped columns: `ID`, `Case Number`, `Description`, `X Coordinate`, `Y Coordinate`, `Location`.
- **Reason:** These columns were not contributing to trend-based crime analysis, where time is the most significant factor.

### 5️⃣ Date and Time Feature Engineering

- Split the **Date** column into separate **Date** and **Time** columns.
- Created additional time-based features:
  - **Month**
  - **Week**
  - **Hour**
  - **Season**
  - **Is Weekend**

---

## 📊 Exploratory Data Analysis (EDA)

Performed an in-depth analysis in **Power BI**, uncovering key insights:

1️⃣ **Arrest Rate vs Crime Increase:**

- Found that lower arrest rates correlate with an increase in crime.

2️⃣ **Narcotics Addiction Trend:**

- Narcotics-related crimes have surged in the years **2023** and **2024**.
- Theft crimes are often linked to narcotics acquisition, escalating into violent crimes like homicide.

3️⃣ **Crime Timing Patterns:**

- The **evening hours** and around **midnight (12 AM)** have the highest theft rates.

4️⃣ **Seasonal Trends:**

- Crime rates peak during misty seasons such as **Spring** and **Fall**.

---

## 📝 Recommendations

- 📢 Increase **awareness campaigns** about narcotics abuse.
- 🚓 Enhance police **beat patrols** in identified crime clusters.
- 💼 Allocate **special budgets** to control drug-related activities.
- 🏥 Establish more **drug relief centers**.
- 📹 Install **security cameras** on streets and sidewalks.
- 🌙 Encourage people to **avoid late-night outings**.
- 🥋 Promote **self-defense training** among community members.

---

## 🏁 Conclusion

This analysis highlights critical crime trends and provides actionable recommendations for improving public safety. By addressing narcotics addiction, increasing surveillance, and empowering communities, significant progress can be made in reducing crime rates.

---

## 📂 Repository Structure

- **/data:** Contains raw and cleaned datasets.
- **/notebooks:** VISUAL STUDIO notebooks for preprocessing and analysis.
- **/reports:** EDA reports and visualizations.
- **/README.md:** Project overview and documentation.

## 📧 Contact

For any questions or collaborations, feel free to reach out!

**Author:** REBINFERNART.K\
**Email:** [krebinfernart@gmail.com](mailto\:krebinfernart@gmail.com)

---

**⭐ If you found this project helpful, don't forget to star this repository!**

