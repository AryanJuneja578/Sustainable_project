# Sustainable_project
# Sustainable Building Energy Consumption Analysis

## Project Overview

This project analyzes building energy consumption patterns and groups buildings into different categories using Machine Learning techniques. The goal is to identify energy usage behavior, detect inefficiencies, and provide actionable recommendations for improving sustainability and energy efficiency.

The project uses:

- Data Preprocessing
- Exploratory Data Analysis (EDA)
- Feature Engineering
- Principal Component Analysis (PCA)
- K-Means Clustering
- Data Visualization
- Energy Optimization Recommendations

---

## Problem Statement

Buildings consume a significant portion of global energy resources. Understanding consumption patterns can help reduce energy waste, lower costs, and improve sustainability.

This project aims to:

- Analyze building energy usage data.
- Identify hidden consumption patterns.
- Cluster buildings with similar energy behavior.
- Generate recommendations for energy optimization.

---

## Dataset Features

The dataset contains timestamp-based building energy consumption information.

Key attributes used:

- Building_ID
- Timestamp
- Energy_Usage (kWh)

Additional engineered features:

- Peak Demand
- Average Load
- Load Variability
- Night Load
- Day Load
- Weekend Load

---

## Project Workflow

### 1. Data Preprocessing

- Loaded the dataset using Pandas.
- Checked data types and missing values.
- Converted timestamps into datetime format.
- Extracted:
  - Hour
  - Day of Week

### 2. Exploratory Data Analysis (EDA)

- Distribution analysis of energy consumption.
- Outlier detection using box plots.
- Statistical summaries of energy usage.

### 3. Feature Engineering

Created building-level energy metrics:

| Feature | Description |
|----------|-------------|
| Peak_Demand | Maximum energy usage |
| Avg_Load | Average energy consumption |
| Load_Variability | Standard deviation of usage |
| Night_Load | Average usage during 12 AM–5 AM |
| Day_Load | Average usage during working hours |
| Weekend_Load | Average usage during weekends |

### 4. Data Standardization

Features were scaled using StandardScaler to ensure equal contribution during clustering.

### 5. Principal Component Analysis (PCA)

PCA was applied to:

- Reduce dimensionality
- Remove redundancy
- Preserve major variance in data

Three principal components were retained for clustering and visualization.

### 6. K-Means Clustering

K-Means clustering was used to group buildings based on energy behavior.

Methods used for selecting optimal clusters:

- Elbow Method
- Silhouette Score

Final number of clusters selected:

**K = 3**

---

## Cluster Interpretation

### Cluster 0
**Night-Heavy & Variable Buildings**

Characteristics:
- High nighttime energy consumption
- Significant variability in usage

Recommendations:
- Implement automated shutdown systems
- Use occupancy sensors
- Apply load smoothing techniques
- Detect abnormal nighttime spikes

---

### Cluster 1
**High-Usage Daytime & Weekend Buildings**

Characteristics:
- Heavy daytime energy consumption
- Significant weekend activity

Recommendations:
- Optimize HVAC operations
- Improve daylight utilization
- Participate in demand-response programs
- Optimize weekend schedules

---

### Cluster 2
**Energy-Efficient & Stable Buildings**

Characteristics:
- Consistent and efficient energy usage
- Lower variability

Recommendations:
- Maintain current efficiency standards
- Use as benchmark buildings
- Implement advanced monitoring
- Integrate renewable energy sources

---

## Visualizations

The project includes:

- Energy Usage Distribution
- Outlier Detection Boxplots
- PCA Scree Plot
- Elbow Method Graph
- Silhouette Score Analysis
- Cluster Distribution Count Plot
- 3D PCA Cluster Visualization
- Cluster-wise Feature Comparison
- Average Energy Feature Analysis

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn

---

## Machine Learning Techniques

- Feature Engineering
- Standardization
- Principal Component Analysis (PCA)
- K-Means Clustering
- Silhouette Analysis

---

## Key Outcomes

- Identified distinct building energy consumption patterns.
- Reduced feature complexity using PCA.
- Segmented buildings into meaningful energy behavior clusters.
- Generated targeted recommendations for energy efficiency improvements.
- Demonstrated how unsupervised learning can support sustainable energy management.

---

## Future Improvements

- Real-time energy monitoring dashboards.
- Predictive energy consumption forecasting.
- Integration with IoT sensor data.
- Automated anomaly detection.
- Renewable energy optimization strategies.

---

## Author

Aryan Juneja

Computer Engineering Student | Data Analytics & Machine Learning Enthusiast
