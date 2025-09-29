# 🏃 EDA Marathon Project

Exploratory Data Analysis (EDA) of **ultra-marathon running dataset**, with a specific focus on the **Trail Du Ventoux 46 km event in France**.  
The goal of this analysis is to explore the dataset, clean and preprocess the data, and uncover meaningful insights about runner demographics and performance in this event.

📊 **Dataset source:** [Kaggle - The Big Dataset of Ultra Marathon Running](https://www.kaggle.com/datasets/aiaiaidavid/the-big-dataset-of-ultra-marathon-running)

---

## 📌 Project Objectives
1. Identify and extract data for the **Trail Du Ventoux 46 km** event held in 2018.  
2. Perform **data preprocessing**: cleaning, formatting, handling missing values, and removing duplicates.  
3. Explore runner demographics (age, gender) and performance statistics.  
4. Visualize performance distribution to understand trends in **speed, age, and gender**.  
5. Identify the **fastest runner** in the event.  

---

## ⚙️ Data Preprocessing
Steps performed before analysis:

- **Data Filtering**  
  Extracted only the rows where `race_name = 'Trail Du Ventoux 46 km'`.  

- **Date Formatting**  
  Converted `race_day` into proper datetime format for easier manipulation.  

- **Removing Duplicates**  
  Checked and removed duplicate race entries.  

- **Data Cleaning**  
  Standardized column names and formatted race distance (`46 km` → `46km`) for consistency.  

- **Feature Engineering**  
  Derived new insights such as **average speed distribution** and segmented runners by **age** and **gender**.

---

## 📊 Exploratory Analysis & Visualizations

### 1. Number of Participants  
- The **Trail Du Ventoux 46 km** event had **893 finishers** in 2018.  
- Using `sns.histplot`, we confirmed the race distance distribution (all finishers ran the 46 km race).  

---

### 2. Gender Distribution  
- Visualization shows that the majority of participants were **male runners (M)** compared to females (F).  
- This highlights the gender imbalance in ultra-marathon participation.

---

### 3. Average Speed Distribution  
- Histogram of `athlete_average_speed` reveals most runners had an **average pace between 6–8 km/h**.  
- The distribution is slightly right-skewed, showing a small number of very fast athletes.  

---

### 4. Gender vs Speed  
- Violin plots showed **males generally had higher average speeds** compared to females.  
- However, the spread of performance overlaps, indicating strong performances across both genders.

---

### 5. Age vs Speed Correlation  
- Scatter plot analysis (with regression line) showed a **negative correlation between age and speed**.  
- Younger athletes tended to run faster, while older athletes showed lower average speeds.  
- Both genders follow a similar trend.

---

## 🏅 Key Insights
1. The **fastest runner** completed the 46 km race in **~4 hours**, with an average speed of **>11 km/h**.  
2. Majority of runners finished between **6–8 km/h**, showing endurance but not sprint-level speeds.  
3. Male participation dominated the event, though female runners showed competitive performance.  
4. Performance tends to decline with age, but experienced athletes still maintained solid endurance across different age groups.  

---

## 📌 Technologies Used
- **Python**
- **Pandas & NumPy** – Data preprocessing
- **Matplotlib & Seaborn** – Visualization
- **Jupyter Notebook** – Analysis workflow

---
