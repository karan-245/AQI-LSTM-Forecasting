# AQI Forecast Using LSTM

A Streamlit-based **Air Quality Index (AQI) prediction system** that uses **LSTM (Long Short-Term Memory) deep learning** to forecast future air pollution levels for any city.

The application fetches **real-time historical PM2.5 data**, converts it to AQI, predicts **future AQI values**, classifies pollution levels, and visualizes results using interactive charts and maps.

---

# Features

*  **City-Based AQI Prediction**
  Enter any city name and get AQI analysis.

*  **7-Day AQI Forecast**
  Uses an **LSTM deep learning model** to predict future AQI.

*  **AQI Trend Visualization**
  Displays historical AQI and predicted AQI on a time-series graph.

*  **AQI Category Distribution**
  Shows how many days fall under different AQI categories.

*  **AQI Map of India**
  Displays AQI levels of major Indian cities on an interactive map.

* 🛰️ **Satellite Pollution Visualization**
  Shows geographic location of the selected city.

*  **AQI Classification Table**
  Provides AQI ranges and their health impacts.

*  **Model Evaluation Metrics**

  * MAE (Mean Absolute Error)
  * RMSE (Root Mean Squared Error)

---

#  Machine Learning Model

This project uses a **Long Short-Term Memory (LSTM)** neural network for time-series prediction.

### Model Architecture

Input → LSTM (64 units) → Dropout → LSTM (32 units) → Dense → AQI Prediction

The model learns patterns from **365 days of historical PM2.5 data** and forecasts the next **7 days AQI**.

---

#  Data Source

Air quality data is fetched from:

**Open-Meteo Air Quality API**

* PM2.5 hourly data
* Converted to daily averages
* Converted to AQI using EPA formula

API:
https://air-quality-api.open-meteo.com

---

# 🛠️ Technologies Used

| Technology         | Purpose                     |
| ------------------ | --------------------------- |
| Python             | Programming Language        |
| Streamlit          | Web Application Framework   |
| TensorFlow / Keras | Deep Learning Model         |
| Scikit-learn       | Data scaling and evaluation |
| Pandas             | Data processing             |
| NumPy              | Numerical operations        |
| Matplotlib         | Visualization               |
| PyDeck             | Interactive AQI map         |
| Open-Meteo API     | Air Quality Data            |

---

# 📊 AQI Classification

| AQI Range | Category        | Health Impact                             |
| --------- | --------------- | ----------------------------------------- |
| 0–50      | Good 🟢         | Minimal impact                            |
| 51–100    | Satisfactory 🟡 | Minor discomfort                          |
| 101–200   | Moderate 🟠     | Breathing discomfort for sensitive people |
| 201–300   | Poor 🔴         | Breathing discomfort to most people       |
| 301–400   | Very Poor 🟣    | Respiratory illness possible              |
| 401–500   | Severe ⚫        | Serious health effects                    |

---


