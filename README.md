# AI-Powered-Smart-Data-Insights-App-

Overview

This project is a web-based data analytics application that allows users to upload a CSV file and automatically generate basic business insights such as revenue metrics, trends, category-wise analysis, and anomaly detection.

The backend is built using FastAPI and runs on Google Cloud Run. Data processing and aggregation are handled using BigQuery, and natural-language insights are generated using Vertex AI.

Problem Statement

Analyzing large datasets manually is time-consuming and requires technical expertise. Many users struggle to quickly understand trends, key metrics, and unusual patterns in their data.

This project aims to simplify data analysis by providing an automated system that converts raw CSV data into structured insights and summaries.

Solution

The application provides:

CSV upload support

Automatic data loading into BigQuery

KPI calculation using SQL

Trend and category analysis

Basic anomaly detection

AI-generated text summary of insights

All processing happens on the cloud, making the system scalable and easy to use.

Key Features

Upload CSV files through a web interface

Calculate total revenue, total units sold, and total orders

Revenue trend visualization

Category-wise revenue breakdown

Anomaly detection using statistical methods

AI-generated insight summary

Cloud-native deployment using Google Cloud Run

Tech Stack

Backend

Python

FastAPI

Data & AI

Google BigQuery

Google Cloud Storage

Vertex AI (Gemini)

Frontend

HTML

CSS

JavaScript

Cloud

Docker

Google Cloud Run

Google Cloud Build

Project Structure
AI-Powered-Smart-Data-Insights-App
│
├── frontend/
│   ├── index.html        # Frontend UI
│
├── main.py               # FastAPI backend logic
├── requirements.txt      # Python dependencies
├── Dockerfile            # Docker configuration
├── README.md

CSV File Requirements

The uploaded CSV file must contain the following columns:

order_id
order_date
region
product_category
units_sold
unit_price


Example:

order_id,order_date,region,product_category,units_sold,unit_price
101,2025-01-01,North,Electronics,2,15000
102,2025-01-02,South,Clothing,5,1200

How the Application Works

User uploads a CSV file

File is stored in Google Cloud Storage

Data is loaded into BigQuery

SQL queries generate metrics and trends

Anomaly detection is applied on daily revenue

Vertex AI generates a text-based summary

Results are displayed on the dashboard

Deployment

The application is containerized using Docker and deployed on Google Cloud Run for scalability and availability.

Use Cases

Business data analysis

Sales performance tracking

BI and analytics demos

Academic and portfolio projects

Author

Mohammad Rehaan Ali
B.Tech CSE (Data Science)


Cloud deployment

Real data processing
