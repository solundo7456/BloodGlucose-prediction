🩸 #Blood Glucose Prediction Using LSTM Neural Networks
📌 ## Project Overview

This project focuses on short-term blood glucose prediction using Long Short-Term Memory (LSTM) neural networks applied to DiaTrend continuous glucose monitoring (CGM) data.
The goal is to predict blood glucose levels one hour ahead for a single individual, contributing toward personalized and data-driven diabetes management.

Physiological time-series data are inherently noisy and non-stationary. To address this, the project involved careful feature engineering, data scaling, and extensive model experimentation to identify an optimal predictive architecture.

🎯 Objectives

Predict blood glucose values 60 minutes into the future

Capture temporal glucose dynamics using LSTM networks

Improve prediction accuracy through feature engineering and normalization

Compare multiple LSTM configurations and select the best-performing model

🧠 Data Processing & Feature Engineering

Significant preprocessing was performed to improve model performance:

Feature engineering to structure glucose sequences suitable for time-series modeling

Creation of sliding windows to capture temporal dependencies

Scaling/normalization of glucose values to stabilize training and improve convergence

Careful handling of sequential input-output alignment for one-hour-ahead prediction

These steps were critical in improving learning stability and predictive accuracy.

🧪 Model Development & Experimentation

Multiple LSTM architectures were trained and evaluated

Hyperparameters explored included:

Number of hidden units

Dropout rates

Learning rates

Batch sizes

Sequence lengths

Models were trained for 30 epochs, with performance monitored across epochs

The best-performing configuration was selected based on validation performance

⚙️ Best Model Configuration

The optimal LSTM model used the following hyperparameters:

(hidden_units, dropout, learning_rate, batch_size, sequence_length)
(32, 0.2, 0.001, 64, 12)

📊 Performance Metrics

The final model achieved the following results on the test set:

Mean Squared Error (MSE): 0.0027

Mean Absolute Error (MAE): 0.0358

R² Score: 0.8544

These results demonstrate strong short-term predictive performance and effective modeling of glucose trends.

💾 Model Output

Best model saved as:
glucose_lstm_best_model.pt

Training showed consistent performance improvement, indicating stable learning and good generalization.

🔬 Key Learnings

This project provided practical experience in:

Feature engineering for physiological time-series data

Scaling and normalization strategies for neural networks

Systematic comparison of deep learning architectures

Translating machine learning performance into clinically meaningful insights

It highlights how iterative model experimentation and thoughtful data preparation are essential for applying AI in healthcare contexts.
