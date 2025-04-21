# README.md

## 📊 Stakeholder Engagement Level Detection

This project provides a machine learning-powered solution to assess stakeholder engagement levels and their corresponding risk levels using synthetic data. The app is designed for project managers, sustainability analysts, and data scientists interested in stakeholder dynamics and project risk management.

---

### 🔧 Components

- **`train_rf_model.py`** – Generates synthetic data and trains a Random Forest classifier.
- **`streamlit_app.py`** – Streamlit dashboard for interactive prediction.
- **Risk Mapping Function** – Maps predicted engagement levels (Low, Medium, High) to risk scores.

---

### 🗂️ File Structure
```
stakeholder_engagement/
│
├── models/
│   └── rf_model.pkl                  # Trained RF model
│
├── app/
│   └── streamlit_app.py              # Main dashboard
│
├── data/
│   └── sample_stakeholders.csv       # Example stakeholder input
│
├── train_rf_model.py                # Model training script
├── README.md                        # This file
```

---

### 🚀 How to Use
1. **Install dependencies**
```bash
pip install pandas scikit-learn streamlit joblib
```

2. **Train the model**
```bash
python train_rf_model.py
```

3. **Run the dashboard**
```bash
streamlit run app/streamlit_app.py
```

4. **Upload stakeholder CSV** with the following format:
```csv
communication_freq,meeting_attendance,feedback_quality,responsiveness
5,80,4,5
3,60,2,2
...
```

---

### 📈 Engagement Levels & Risk Scores
| Engagement Level | Risk Score | Description          |
|------------------|------------|----------------------|
| High             | 0.2        | Low risk, proactive  |
| Medium           | 0.5        | Moderate risk        |
| Low              | 0.8        | High risk, inactive  |

---

### 📌 To-Do (Next Phase)
- [ ] Add LSTM model for temporal tracking.
- [ ] Deploy as a web app (e.g., Streamlit Cloud).
- [ ] Add CSV export of results.

---

### 👨‍💻 Author
Developed by [Geosoft Global Innovation Ltd.](https://github.com/Akajiaku1) | Powered by synthetic ML and stakeholder science.
