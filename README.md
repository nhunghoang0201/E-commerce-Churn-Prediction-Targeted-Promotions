# E-commerce-Churn-Prediction-Targeted-Promotions
Author: Hoang Thi Hong Nhung  
Date: 2925-09-03  
Tools Used: Python

## 📑 Table of Contents  
1. [📌 Background & Overview](#-background--overview)  
2. [📂 Dataset Description & Data Structure](#-dataset-description--data-structure)  
3. [🔎 Final Conclusion & Recommendations](#-final-conclusion--recommendations)

## 📌 Background & Overview  
#### Objective
Predict which users will churn for an e-commerce company and design promotion strategies to reduce churn.

📖 What is this project about? What Business Question will it solve?

Build a churn prediction model from user profile, behavior, and engagement signals.

Explain drivers of churn (patterns/behaviors).

Segment churned users for targeted promotions (personalized retention offers).

Main business questions:

Who is likely to churn next month?

Why do users churn (key features/behaviors)?

What promotions should we offer to each churned segment?

#### 👤 Who is this project for?
✔️ Data & ML teams in e-commerce/marketplaces
✔️ Market/Growth teams (retention, win-back)

## 📂 Dataset Description & Data Structure  
#### 📊 Tables Used
The dataset contains 1 table: Customer Churn Features

#### Table definition & Data Snapshot
| Column Name                 | Type  | Description                              |
| --------------------------- | ----- | ---------------------------------------- |
| CustomerID                  | INT   | Unique customer ID                       |
| Churn                       | INT   | Churn flag (1 = churned)                 |
| Tenure                      | INT   | Months with company                      |
| PreferredLoginDevice        | TEXT  | Login device (Mobile Phone, Computer)    |
| CityTier                    | INT   | City tier (1/2/3)                        |
| WarehouseToHome             | INT   | Distance from warehouse to home          |
| PreferredPaymentMode        | TEXT  | E wallet / Debit Card / COD…             |
| Gender                      | TEXT  | Male/Female                              |
| HourSpendOnApp              | INT   | Hours spent on app/site                  |
| NumberOfDeviceRegistered    | INT   | Registered devices count                 |
| PreferedOrderCat            | TEXT  | Last month’s preferred order category    |
| SatisfactionScore           | INT   | Customer satisfaction (e.g., 1–5)        |
| MaritalStatus               | TEXT  | Single/Married/Divorced                  |
| NumberOfAddress             | INT   | Number of saved addresses                |
| Complain                    | INT   | Complaint raised last month (0/1)        |
| OrderAmountHikeFromlastYear | INT   | % increase in order amount vs. last year |
| CouponUsed                  | INT   | Coupons used last month                  |
| OrderCount                  | INT   | Orders placed last month                 |
| DaySinceLastOrder           | INT   | Days since last order                    |
| CashbackAmount              | FLOAT | Avg cashback last month                  |

| CustomerID | Churn | Tenure | PreferredLoginDevice | CityTier | WarehouseToHome | PreferredPaymentMode | Gender | HourSpendOnApp | NumberOfDeviceRegistered | PreferedOrderCat   | SatisfactionScore | MaritalStatus | NumberOfAddress | Complain | OrderAmountHikeFromLastYear | CouponUsed | OrderCount | DaySinceLastOrder | CashbackAmount |
| ---------- | ----- | ------ | -------------------- | -------- | --------------- | -------------------- | ------ | -------------- | ------------------------ | ------------------ | ----------------- | ------------- | --------------- | -------- | --------------------------- | ---------- | ---------- | ----------------- | -------------- |
| 52869      | 0     | 20     | Mobile Phone         | 3        | 7               | E wallet             | Female | 4              | 4                        | Fashion            | 5                 | Married       | 3               | 0        | 26                          | 5          | 16         | –                 | 230            |
| 52942      | 0     | 13     | Computer             | 1        | 9               | Cash on Delivery     | Female | 4              | 4                        | Fashion            | 3                 | Single        | 2               | 0        | 26                          | 11         | –          | 9                 | 234            |
| 52972      | 0     | 16     | Mobile Phone         | 3        | 7               | Debit Card           | Male   | 3              | 4                        | Laptop & Accessory | 3                 | Divorced      | 3               | 0        | 26                          | 5          | 12         | 7                 | 174            |
| 53125      | 0     | 5      | Mobile Phone         | 1        | 16              | Debit Card           | Male   | 3              | 4                        | Fashion            | 4                 | Married       | 3               | 0        | 26                          | 2          | 2          | 9                 | 231            |
| 53367      | 0     | 9      | Mobile Phone         | 1        | 28              | Debit Card           | Female | 3              | 4                        | Laptop & Accessory | 2                 | Divorced      | 3               | 1        | 26                          | 1          | 2          | 8                 | 165            |

## ⚒️ Main Process
1️⃣ Data Cleaning & Preprocessing & EDA
2️⃣ Feature Engineering
3️⃣ Modeling
3️⃣ Evaluate model
