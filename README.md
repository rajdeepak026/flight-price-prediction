# ✈️ Flight Price Prediction

This project focuses on predicting flight ticket prices using a real-world dataset. The dataset includes various features such as airline, route, time of travel, and more. The goal is to explore, preprocess, and extract meaningful insights to support future machine learning models for price prediction.

---

## 📂 Dataset Overview

- **Total Records:** 9,450  
- **Total Features:** 13  
- **Target Variable:** `Price`

### 📌 Columns Description

| Column Name       | Description                                      |
|-------------------|--------------------------------------------------|
| Airline           | Name of the airline                              |
| Source            | Flight departure location                        |
| Destination       | Flight arrival location                          |
| Route             | The route taken by the flight                    |
| Dep_Time          | Departure time                                   |
| Arrival_Time      | Arrival time                                     |
| Duration          | Total flight duration                            |
| Total_Stops       | Number of stops                                  |
| Additional_Info   | Extra information about the flight               |
| Price             | 💰 Target variable – ticket price                |
| Month             | Month of journey                                 |
| WeekDay           | Day of the week of travel                        |
| Day               | Date of the journey                              |

---

## 📊 Key Insights

- **Average Price:** ₹9027.90  
- **Busiest Month:** May  
- **Higher Prices:** On **weekends** (Saturday & Sunday)  
- **Most Frequent Travel Day:** Wednesday  
- **Flights with Airline 'IndiGo' & 'No info':** 1650  
- **Average Duration:** ~38,958 seconds (~10.8 hours)  

---

## ⚙️ Data Preprocessing & Feature Engineering

- Cleaned inconsistent entries (e.g., 'No Info' → 'No info')
- Converted `Duration` from text to seconds
- Extracted **Hour** from `Dep_Time` and `Arrival_Time`
- Created **Time of Day Categories**:
  - Morning (5–11)
  - Afternoon (12–16)
  - Evening (17–19)
  - Night (20–4)
- Encoded `WeekDay` as binary:  
  - `1` → Weekend  
  - `0` → Weekday

---

## 🛠️ Technologies Used

- Python 🐍
- Pandas
- NumPy
- Google Colab

---

## 📁 Project Structure

