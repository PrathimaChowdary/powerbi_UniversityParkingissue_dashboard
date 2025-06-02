# University – Parking Access Analytics Dashboard (Power BI)

This Power BI project analyzes parking access patterns at the University, using card transaction data from January 2021 to April 2025. It provides insights into peak usage times across gated parking lots, user behavior, and forecasting future lot usage to support better access group assignments and resource planning.

## Download Power BI File
##[Click here to download the Power BI report]
https://drive.google.com/file/d/1uaBzNDN81sRGrVQrIlf554Nnzo6JIZuD/view?usp=drive_link

## 🎯 Objective

To assist the University Parking & Transportation Department in:
- Understanding **parking space utilization**
- Identifying **peak usage periods** at lot, daily, weekly, and monthly levels
- Supporting data-driven decisions for **issuing new access cards**
- Forecasting **future lot demand** for the remainder of 2025


## 📁 Dataset Description

### 1. **CardAccessGroupAssignment**
- Maps **Card Numbers** to their respective **Access Groups**
- Access groups determine which lots a card can access, subject to priority rules

### 2. **CardTransaction**
Contains all transactions from Jan 1, 2021 – Apr 30, 2025:
- `TransactionId`: Unique ID
- `CardNumber`, `LotNumber`
- `EntranceTime`, `ExitTime` *(missing times default to midnight before/after)*
- `NoEntry`, `NoExit`, `Overnight`: Binary flags
- `EffectiveGroupNumber`: Access group used to authorize the transaction


## 🧠 Key Logic & Assumptions

- Missing `EntranceTime` assumed to be **midnight before** `ExitTime`
- Missing `ExitTime` assumed to be **midnight after** `EntranceTime`
- Lot usage is measured by **duration between Entrance and Exit**
- Peak usage is defined as the **maximum simultaneous occupancy** in each lot per day/week/month


## 📊 Dashboard Features

- 🚗 **Lot Utilization Trends**: Daily, Weekly, Monthly summaries
- ⏰ **Peak Usage Timeline**: Lot-wise peak usage and simultaneous occupancy charts
- 🧭 **Access Group Effectiveness**: Analyze how card assignments impact lot usage
- 📈 **Forecasting (2025)**: Predict peak periods for the remaining months of 2025
- 🔍 **Filters**: Dynamic filters by Lot, Time Period, and Access Group


## 🖼️ Dashboard Preview

![Dashboard Screenshots] <img width="956" alt="image" src="https://github.com/user-attachments/assets/a0e1ef8d-9d44-427d-8253-5d35db574f4d" />   <img width="959" alt="image" src="https://github.com/user-attachments/assets/77529ed9-3c86-45b9-9240-248d456e131c" />  <img width="957" alt="image" src="https://github.com/user-attachments/assets/03d86b1a-08af-4fc6-b4e2-c5c72148ec4e" />  <img width="959" alt="image" src="https://github.com/user-attachments/assets/8fc27050-99ee-44b5-bdde-a8570578f6c5" /> 






## ⚙️ Tools & Technologies

- **Power BI Desktop**
- **DAX** for time intelligence and measure calculations
- **Power Query** for ETL transformations
- Forecasting using **built-in analytics tools** in Power BI

## 📌 Additional Considerations

- Academic calendar and special events may affect parking patterns
- Cards added or reassigned to new Access Groups during the data window may show shifted behavior


## 📬 Contact

For questions or collaboration opportunities:

- 👩‍💼 Name: Prathima Chowdary
- 📧 Email: chowdaryprathima707@gmail.com
- 💼 LinkedIn: https://www.linkedin.com/in/devineni-prathima-4b5538213/


– University Parking Data Analytics


