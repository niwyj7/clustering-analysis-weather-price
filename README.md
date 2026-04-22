# Power Market Clustering Analysis

##  Overview

The project focuses on extracting patterns from high-dimensional energy data. By using **DBSCAN (Density-Based Spatial Clustering of Applications with Noise)**, the model can group similar market days/hours together while automatically filtering out market anomalies as noise.

##  Features

- **Automated Parameter Optimisation**: Includes an improved logic (`find_optimal_dbscan_params_improved`) that uses $k$-distance graphs and elbow-point detection to find the ideal `eps` and `min_samples` for DBSCAN.
- **Advanced Preprocessing**:
    - Handling of holidays via the `chinese_calendar` library.
    - Robust scaling and outlier removal using Z-score and `StandardScaler`.
- **Dimensionality Reduction**: Implements **t-SNE** (t-Distributed Stochastic Neighbour Embedding) to visualise high-dimensional energy clusters in a 2D space.
- **Market Impact Analysis**: Correlates identified clusters with price spreads and solar generation forecasts.

## visualise cluster price spread
<img width="2390" height="590" alt="image" src="https://github.com/user-attachments/assets/92fae00b-5e09-458a-aa79-6bd3348b8089" />


