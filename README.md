# Analytics-QA-Engineer-Intern---Technical-Project-Brief

# Performance Analysis Dashboard

## Project Overview
This project involves creating a Python-based dashboard to analyze app performance metrics using log data. The analysis includes calculating key metrics, visualizations, and anomaly detection to monitor app health effectively.

---

## Key Features
- **Metrics Calculation**:
  - Average and 95th Percentile (P95) Response Times
  - Error Rates and Types
  - Peak Usage Periods
  - User Experience Metrics (e.g., % of requests > 1s)

- **Visualizations**:
  - Response Time Trends
  - Error Rate Patterns
  - Endpoint Performance Comparison
  - Peak Usage Analysis

- **Anomaly Detection**:
  - Identifying spikes in response time
  - Detecting unusual error rate patterns

---

## Setup Instructions
1. **Install Python 3.8+**.
2. **Install required libraries**:
   ```bash
   pip install pandas matplotlib seaborn numpy
   
## Run the script/notebook:
Open the performance_analysis.ipynb in Google Colab or Jupyter Notebook.
Ensure the dataset (logs.csv) is in the same directory as the script.

## Approach
Data Preprocessing:

Converted timestamps to a usable format.
Cleaned and validated the dataset.
Metrics Calculation:

Grouped data by endpoint and hour for aggregations.
Calculated advanced metrics like P95 response times.
Visualizations:

Used matplotlib and seaborn for clear and interactive charts.
Anomaly Detection:

Defined thresholds using mean and standard deviation.

## Key Insights
Certain endpoints have significantly higher P95 response times.
Peak usage occurs between 8 PM and 10 PM.
Most errors are related to HTTP 500 status codes, indicating server issues.
Around 15% of requests take longer than 1 second, suggesting room for optimization.

## Future Improvements
Implement a more robust anomaly detection algorithm (e.g., using machine learning).
Use an interactive dashboard library like Plotly or Dash for better user experience.
Incorporate real-time monitoring capabilities with live data feeds.
