# DNS Log Analysis and Anomaly Detection

## Overview
This project focuses on analyzing DNS logs to identify and classify different log types, enabling efficient detection of potential anomalies or threats in network traffic. The analysis leverages machine learning models such as Random Forest, KNN, and Decision Tree to achieve high accuracy and actionable insights.

## Features
- **Data Preprocessing**: Cleanses and prepares raw DNS log data for analysis.
- **Feature Engineering**: Extracts critical features such as `category`, `client_ip`, and `query` for model training.
- **Model Training and Evaluation**: Implements multiple machine learning models with detailed performance metrics.
- **Visualization**: Provides intuitive visualizations for feature importance, log distributions, and model performance.
- **Feature Insights**: Identifies key features that contribute most to anomaly detection.

## Key Metrics
| **Model**         | **Accuracy (%)** | **Precision (%)** | **Recall (%)** | **F1-Score (%)** |
|--------------------|------------------|-------------------|----------------|------------------|
| **Random Forest**  | 95.8            | 95.8             | 97.7           | 97.5             |
| **KNN**            | 99.38           | 98.86            | 99.0           | 93.1             |
| **Decision Tree**  | 95.4            | 93.1             | 95.46          | 97.42            |

## Approach
1. **Data Extraction**: Logs are parsed to extract features like date, time, client IP, and query.
2. **Feature Encoding**: Categorical features are encoded using Label Encoding for machine learning compatibility.
3. **Model Training**: 
   - **Random Forest**: Robust to noise and emphasizes critical features.
   - **KNN**: Classifies based on proximity in feature space.
   - **Decision Tree**: Provides interpretable decision-making splits.
4. **Evaluation**: Models are assessed on Accuracy, Precision, Recall, and F1-Score.

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/dns-log-analysis.git
2. Navigate to the project directory:
```bash
  cd dns-log-analysis
```
3. Copy code
```bash
  pip install -r requirements.txt
```
4. Usage
```
Place your DNS log file (log.csv) in the project directory.
```
5. Run the analysis script:
```bash 
  python analyze_logs.py
```
## Visualizations
1. **Confusion Matrices**: Highlight model accuracy for each class.
2. **Feature Importance**: Visualizes the contribution of each feature.
3. **Log Distributions**: Explores patterns and anomalies over time.
## Future Scope
1. **Scalability**: Extend analysis to larger datasets for enterprise-scale networks.
2. **Real-Time Analysis**: Implement a streaming pipeline for real-time anomaly detection.
3. **Advanced Models**: Explore deep learning models for higher accuracy on complex patterns.
