# 🌱 Crop Recommendation using IBM Watson AutoAI

This project predicts the most suitable crop to grow based on soil and weather conditions using **IBM Watson AutoAI**.

## 📊 Dataset

- File: `crop_recommendation.csv`
- Features used:
  - N (Nitrogen)
  - P (Phosphorus)
  - K (Potassium)
  - Temperature (°C)
  - Humidity (%)
  - pH
  - Rainfall (mm)
  - **Label**: Crop name (e.g., rice, maize, etc.)

## 🔧 Tools Used

- IBM Watson AutoAI (GUI-based model training)
- IBM Watson Machine Learning (for deployment)
- No code was written — entire model creation and deployment were done using AutoAI GUI.

## 🚀 Deployment

The model was deployed on IBM Watson. Once deployed, it provided a REST API endpoint to send input values and receive crop predictions.

## 📥 Example Input (Scoring Payload)

```json
{
  "input_data": [
    {
      "fields": ["N", "P", "K", "temperature", "humidity", "ph", "rainfall"],
      "values": [[90, 42, 43, 20.8, 82.0, 6.5, 202.9]]
    }
  ]
}
