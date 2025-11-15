# Task 2: SmartAgri Simple AI-IoT 🌱🤖

## Overview
This project simulates a **Smart Agriculture system** that integrates **AI and IoT** to predict crop yield and provide simple irrigation recommendations.  

It demonstrates:
- AI-IoT integration
- Edge-style inference
- Human-AI collaboration for decision-making
- Practical use of sensors in agriculture

---

## Folder Structure

Task 2 SmartAgri-Simple-AI-IoT/
│
├── smartagri_model.ipynb # Notebook to train the AI model
├── linear_model_yield.joblib # Trained AI model
├── infer.py # Script for real-time predictions
├── data_flow_diagram.png # Diagram showing data flow from sensors to AI predictions
└── README.md # This file

---

## Sensors Used
- **Soil Moisture Sensor**: Measures soil water content (%)  
- **Temperature Sensor (DHT22 / LM35)**: Measures air/soil temperature (°C)  
- **Light Intensity Sensor (LDR / BH1750)**: Measures sunlight level (lux)  

---

## How It Works
1. **Sensors** collect soil moisture, temperature, and light intensity data.  
2. Data is sent to an **AI model** (simulated here via a notebook or inference script).  
3. The AI predicts **crop yield** based on sensor data.  
4. **Irrigation recommendations** are provided based on soil moisture levels.  

---

## How to Run

### Option 1: Using Jupyter Notebook / Kaggle / Colab
1. Open `smartagri_model.ipynb`.  
2. Run all cells to train the model.  
3. The trained model will be saved as `linear_model_yield.joblib`.

### Option 2: Using Inference Script
1. Place `infer.py` and `linear_model_yield.joblib` in the same folder.  
2. Run the script in a terminal:

```bash
python infer.py
Data Flow

The system follows this data flow:

[Sensors]
   Soil Moisture ----\
   Temperature ------- > [IoT Device / Microcontroller] ---> [AI Model Prediction] ---> [Dashboard / Alerts]
   Light Sensor -----/


You can see the visual diagram in data_flow_diagram.png.

Tools & Libraries

Python 3

Libraries: numpy, pandas, scikit-learn, matplotlib, joblib

Diagram: Draw.io 

Notes

This is a simulated AI-IoT project for educational purposes.

The logic can be applied with real sensors in practical agricultural applications.