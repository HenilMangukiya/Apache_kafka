# Real-Time Stock Market Data Visualization Using Apache Kafka & Google Sheets

## 📌 Project Overview
This project focuses on real-time stock market data streaming, processing, and visualization using **Apache Kafka, Google Sheets, and Grafana**. The system fetches stock market data using the **Google Finance API**, streams it through Kafka, stores it in **Google Sheets**, and then visualizes trends and analytics dynamically using **Grafana**.

## 🚀 Features
- **Real-time Stock Data Streaming** via Apache Kafka.
- **Google Sheets Integration** to store real-time data.
- **Dynamic Stock Selection** from a large list in Grafana.
- **Batch Updates for Visualization** instead of real-time streaming.
- **Customizable Time Span** for stock trends analysis.
- **Additional Stock Data Columns** for better insights.

## 🛠 Tech Stack
- **Apache Kafka** - Real-time data streaming.
- **Python** - Kafka Producer & Consumer implementation.
- **Google Sheets API** - Storage for real-time stock data.
- **Grafana** - Dashboard for data visualization.
- **Jupyter Notebook** - Development environment.

## 🔧 Setup Instructions
## Download Apache kafka from the webiste 
### 1️⃣ Install Dependencies
```sh
pip install kafka-python gspread oauth2client pandas
```
### 2️⃣ Set Up Apache Kafka
- Download and extract Kafka: [Kafka Download](https://kafka.apache.org/downloads)
- Start Zookeeper:
  ```sh
  bin/zookeeper-server-start.sh config/zookeeper.properties
  ```
- Start Kafka Server:
  ```sh
  bin/kafka-server-start.sh config/server.properties
  ```
- Create Kafka Topic:
  ```sh
  bin/kafka-topics.sh --create --topic stock-data --bootstrap-server localhost:9092
  ```

  ### 3️⃣ Configure Google Sheets API
- Create a Google Cloud Project & enable **Google Sheets API**.
- Generate and download `credentials.json`.
- Share the Google Sheet with the service account email.




