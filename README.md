# Automating Cryptocurrency Price Tracking with API

## Project Overview
As an aspiring data analyst fascinated by the speed and volatility of cryptocurrency markets, I wanted to go beyond static reports and explore how real-time data could be captured, stored, and analyzed without manual effort.  
This project is the result of that curiosity — an **end-to-end Python automation pipeline** that fetches live cryptocurrency data from the CoinMarketCap API, processes it, and builds a continuously growing dataset for deeper analysis.

---

## Objective
The aim of this project was to:

- Connect to a cryptocurrency API and fetch real-time market data.  
- Automate data collection at fixed intervals.
- Append new market data to an existing dataset without overwriting history  
- Store and maintain historical data for trend analysis.  
- Perform basic transformations and export clean datasets for visualization or reporting.

---

## Tools & Technologies
- **Python (Jupyter Notebook)** – For API calls, JSON parsing, data cleaning, and automation logic    
- **Pandas** – For data wrangling and analysis.  
- **Requests** – To interact with the API.  
- **Datetime & Time** – For timestamping and scheduling data pulls.  
- **CoinMarketCap API (or equivalent)** – For cryptocurrency market data.  
- **Excel/CSV** – For storing cleaned historical datasets.  
- **GitHub** – Version control and project hosting.

---

## Data & Metrics Captured
The dataset generated tracks essential cryptocurrency market indicators, including:

- **Current Price (USD)** – Real-time valuation per coin  
- **Percentage Change (1h, 24h, 7d, 30d, 60d, 90d)** – Short- and long-term movement tracking  
- **Timestamp** – Recording the exact moment of data capture for time-series analysis  

These metrics form the basis for **trend analysis, volatility assessment, performance comparisons and market forecasting** across cryptocurrencies.
 
---

## Data Processing & Automation Steps
1. **API Integration** – Connected to the crypto price API using an authentication key.  
2. **Data Extraction** – Parsed relevant fields such as name, price, and market cap.  
3. **Timestamp Addition** – Added a timestamp column to track when each record was fetched.  
4. **Automation Loop** – Used a `while True` loop with `time.sleep()` to run the extraction at set intervals.  
5. **Data Storage** – Appended each fetch result to a DataFrame and saved periodically to CSV for historical tracking.  

---

## Data Cleaning & Transformation
Data preparation steps included:

- Parsing nested JSON responses from the API  
- Flattening complex structures into a clean DataFrame  
- Adding a **timestamp** column for time-based analysis  
- Appending new API data to the CSV in “append mode” without overwriting previous entries  
- Ensuring numeric precision for financial data with custom display formatting

---

## Key Business Questions Explored
While the current scope is focused on automation and data collection, the foundation supports answering critical analytical questions such as:

- How do cryptocurrency prices fluctuate over different time intervals?  
- Which coins show the highest volatility in short-term vs. long-term windows?  
- What patterns emerge in price changes over days, weeks, and months?

---

## Example Output

| Name        | % Change 1h | % Change 24h | % Change 7d | % Change 30d | % Change 60d | % Change 90d |
|-------------|-------------|--------------|-------------|--------------|--------------|--------------|
| Bitcoin     | 0.23393     | 1.21329      | 5.29876     | -1.89825     | 14.21818     | 17.61839     |
| Ethereum    | -0.03060    | 7.74511      | 27.73440    | 52.05580     | 82.96039     | 81.49646     |
| XRP         | 1.53029     | 4.85510      | 12.23672    | 10.54983     | 51.46689     | 32.16388     |
| Tether USDt | 0.00723     | -0.01526     | -0.00408    | -0.03121     | -0.05813     | -0.02507     |
| BNB         | 0.89998     | 6.16352      | 12.32972    | 20.98435     | 31.15715     | 31.10689     |
| Solana      | 0.64019     | 14.12749     | 22.23981    | 19.07869     | 36.91520     | 16.08422     |
| USDC        | 0.00600     | -0.02107     | -0.01720    | -0.02373     | -0.01706     | -0.02240     |
| Dogecoin    | 0.87093     | 11.86233     | 24.67956    | 20.31957     | 40.74549     | 9.47016      |

<img width="811" height="616" alt="Screenshot 2025-08-13 174643" src="https://github.com/user-attachments/assets/a132cf9f-33d2-400d-94c4-686ec2005be8" />


---

## Key Takeaways
This project helped me:
- Learn **API integration** and authentication workflows.  
- Implemented a **Python-based automation pipeline** for continuous data collection and repeatable time-series analysis.  
- Manage and clean **time-series financial data**.  
- Understand the basics of **market trend tracking** using automated datasets.

---

## Acknowledgements
Inspired by real-world cryptocurrency tracking systems and data engineering workflows.  
Special thanks to the **CoinMarketCap API documentation** and online Python community resources.

---

## About Me
I’m an **aspiring data analyst**, developing my portfolio through real-world use cases in **finance, procurement, HR, operations, marketing analytics** and many more.

**GitHub** – [Sowmyashree21](https://github.com/Sowmyashree21)
