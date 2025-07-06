# Enhancing Shipment Tracking & Delivery Forecasting

Built a complete ETL + analytics pipeline to predict shipment delivery dates and optimize tracking systems for a global electronics distributor (Tenav). This project integrated real-time scraped tracking data with SAP shipment logs to improve ETA accuracy, uncover delay drivers, and enable proactive logistics decision-making.

## 🚚 Problem Statement

Tenav’s internal SAP estimates lacked logic and were often inaccurate, leading to customer dissatisfaction and delivery inefficiencies. The goal was to build a dynamic, data-driven system that would:

- Predict delivery status (on-time, delayed, early)
- Optimize route & carrier choices
- Provide EDA dashboards and threshold-based alerts

## 🧠 Our Approach

### 🔄 Data Collection & ETL
- Built an end-to-end ETL pipeline combining:
  - SAP shipment records
  - Scraped data from FedEx, UPS, etc. via **RPA bots (UiPath)**
  - Explored **API integrations** and **BeautifulSoup** as alternatives to scraping
- Structured and cleaned the data using **Python (pandas, NumPy)** and **Power BI (DAX)**

### 📊 Exploratory Data Analysis
- Conducted in-depth EDA across:
  - Geographic zones (by zip code, state)
  - Carrier performance and route delays
  - Weather impact on delays and exceptions
  - Real-time delivery status classification
- Identified bottlenecks and pain points across regions and carriers

### 📈 Predictive Modeling
- Built time series forecasting models using:
  - **Prophet**
  - **ARIMA**
  - **XGBoost & Random Forest (for classification of status)**
- Trained models on historical shipment data

### ⚠️ Alerts & Automation
- Built alert thresholds for:
  - Delays beyond expected time
  - Carrier underperformance
  - Weather disruptions
- Automated notifications and dashboard filters in Power BI

## 🎯 Results

- Achieved **0.17 MAE** — typically off by only 1 day in delivery predictions  
- Achieved **97% R²** on our best-performing model  
- Delivered actionable insights around route optimization and carrier selection  
- Enabled the client to proactively manage late deliveries and customer expectations

## 🛠 Tools & Technologies

- **Python** (pandas, NumPy, scikit-learn, Prophet, statsmodels)
- **Power BI** (DAX, Dataflows)
- **UiPath** (for RPA-based scraping)
- **BeautifulSoup** (for HTML scraping)
- **SAP Data Exports**
- **Jupyter Notebooks**, Google Colab

## 🔗 Links

- 🌐 [Portfolio Website](https://krutikasoni.github.io)
- 📂 [Power BI Dashboard / Screenshots](#) *(Add if available)*
- 📁 [Project Report or Slides](#) *(Optional)*

