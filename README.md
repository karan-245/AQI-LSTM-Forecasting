The AQI Forecasting System is a machine learning-based web application that predicts future Air Quality Index (AQI) values using a Long Short-Term Memory (LSTM) neural network.
The system fetches real-time PM2.5 air pollution data from the Open-Meteo API, converts it into standardized AQI values, and forecasts air quality for the next three days. The application also provides model evaluation metrics and interactive visualizations through a Streamlit web interface.

## Features
- Real-time AQI data fetching
- PM2.5 to AQI conversion
- LSTM-based time series forecasting
- 3-day AQI prediction
- Model evaluation using MAE and RMSE
- Interactive Streamlit web interface

---

## Technologies Used
- Python
- Streamlit
- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- TensorFlow (LSTM)

---

## Model Details
- Model: LSTM (Recurrent Neural Network)
- Window Size: 14 days
- Train-Test Split: 80-20
- Evaluation Metrics:
  - MAE (Mean Absolute Error)
  - RMSE (Root Mean Squared Error)

---

## Data Source
Open-Meteo Air Quality API

---

## How to Run Locally

```bash
pip install -r requirements.txt
streamlit run app.py
