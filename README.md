# XAI for Anomaly Detection in Banking

## Overview
This project focuses on **Explainable AI (XAI)** techniques applied to anomaly detection in the banking sector. With the increasing complexity of AI models, especially in sensitive domains such as finance, the need for transparency and interpretability has become critical. This project uses **unsupervised machine learning algorithms** to detect fraudulent transactions and explains the decision-making process behind each detection.

## Algorithms Used
Three unsupervised anomaly detection algorithms were implemented to analyze banking transactions:
- **ECOD** (Empirical Cumulative Distribution-Based Outlier Detection)
- **LOF** (Local Outlier Factor)
- **EIF** (Extended Isolation Forest)

These models detect anomalies in transaction datasets, and XAI techniques are used to explain why certain transactions were flagged as anomalous.

## Explainability Methods
The project employs several explainability techniques to ensure model transparency:
- **Feature Importance**: Determines the contribution of each feature (e.g., transaction amount, user location) to the model's prediction.
- **Z-Score Analysis**: Calculates how much a transaction deviates from the mean, helping to quantify its anomaly score.
- **Correlation Analysis**: Measures the relationship between various features and anomaly detection, providing insights into patterns in the data.

## Datasets
The models were trained and evaluated on **synthetic datasets** simulating real-world banking transactions. Each dataset contains labeled data indicating whether a transaction is anomalous (ECOD, LOF) or a continuous anomaly score (EIF).

## Results
Key insights from the project:
- The **transaction amount** was consistently one of the most influential features in detecting anomalies across all models.
- **Temporal analysis** showed peaks of anomalies during certain periods, highlighting potential fraud patterns.
- Feature importance and correlation analysis provided transparency into why specific transactions were flagged as suspicious.

## Technology Stack
- **Python**: Core language for model development.
- **Pandas & Scikit-learn**: Used for data preprocessing and model implementation.
- **Matplotlib & Seaborn**: Libraries used for data visualization and feature importance plotting.
- **Google Colab**: Used as the development environment for running and visualizing models.

## Visualizations
![Feature Importance](images/feature_importance.png)
![Anomaly Distribution](images/anomaly_distribution.png)

These visualizations help illustrate which features contribute most to anomaly detection and how anomalies are distributed over time.

## Conclusion
This project demonstrates the importance of **Explainable AI** in critical applications such as fraud detection, where understanding model decisions is as important as accuracy. By using XAI techniques, the project ensures that models are transparent, interpretable, and trustworthy.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
