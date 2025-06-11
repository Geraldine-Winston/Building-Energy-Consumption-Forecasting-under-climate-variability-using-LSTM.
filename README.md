# Building Energy Consumption Forecasting under Climate Variability using LSTM

This project applies a Long Short-Term Memory (LSTM) neural network to forecast building energy consumption by incorporating climate variability factors such as temperature and humidity. The model leverages time-series patterns to enhance prediction accuracy, particularly under seasonal changes and daily usage cycles.

## 🔍 Project Overview

- **Objective**: Predict hourly building energy usage using LSTM models.
- **Data Features**: Energy consumption, ambient temperature, humidity, timestamp.
- **Approach**:
  - Preprocess and normalize time-series data.
  - Build and train an LSTM model using TensorFlow/Keras.
  - Evaluate and visualize forecasting performance.

## 📁 Project Structure

```
Building-Energy-Forecasting/
│
├── data/
│   └── building_energy.csv        # Input dataset
├── models/
│   └── lstm_model.h5              # Trained LSTM model
├── figures/
│   ├── loss_plot.png              # Training and validation loss
│   └── prediction_vs_actual.png  # Actual vs predicted values
├── scripts/
│   └── train_lstm.py              # Main training and forecasting script
├── requirements.txt              # Python dependencies
└── README.md                     # Project documentation
```

## 🧪 How to Run

1. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

2. **Prepare your data**
   - Ensure your CSV file is in `data/building_energy.csv`.
   - Columns should include: `timestamp`, `energy_consumption`, `temperature`, `humidity`.

3. **Train and forecast**
   ```bash
   cd scripts
   python train_lstm.py
   ```

4. **Outputs**
   - Trained model in `models/`
   - Evaluation plots in `figures/`

## 📊 Example Visualizations

- `loss_plot.png`: Training vs. validation MSE loss over epochs.
- `prediction_vs_actual.png`: Forecasted energy values compared with actuals (last 200 hours of test set).

## 🔧 Requirements

- pandas
- numpy
- matplotlib
- scikit-learn
- tensorflow

Install them using:
```bash
pip install -r requirements.txt
```

## 🧠 Future Enhancements

- Include additional weather parameters (e.g., wind speed, solar radiation).
- Hyperparameter tuning and model comparison (e.g., GRU, Bi-LSTM).
- Streamlit dashboard for live forecasting.

## 👩‍💻 Author

**Ayebawanaemi Geraldine Winston**  

