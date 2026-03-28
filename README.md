Here is your **README.md** for the *Wildfire Corridor Mapping using GIS and ML-Based Resistance Surfaces* project:

---

# 🔥 Wildfire Corridor Mapping using GIS and Machine Learning

## 📌 Project Overview

This project models potential **wildfire spread corridors** by combining **GIS-based environmental factors** with **machine learning-derived resistance surfaces**. It simulates how fire moves across landscapes by identifying low-resistance pathways influenced by terrain, vegetation, moisture, and human activity.

The workflow demonstrates how spatial analysis and AI can support wildfire risk assessment and landscape management.

---

## 🎯 Objectives

* Simulate environmental GIS layers
* Generate wildfire resistance surfaces
* Train a machine learning model to predict resistance
* Identify least-cost wildfire spread corridors
* Visualize and export wildfire pathways

---

## 🗺 Input Spatial Layers (Synthetic)

* **Slope** – Influences fire spread speed
* **Vegetation Density (NDVI proxy)** – Fuel availability
* **Soil Moisture** – Dampens fire propagation
* **Distance to Roads** – Proxy for human ignition sources

---

## 🔥 Resistance Surface Concept

* **Low resistance** → Easier fire spread
* **High resistance** → Reduced fire movement

The resistance surface is generated using a **Random Forest regression model**, capturing nonlinear relationships between environmental variables and fire spread potential.

---

## 🤖 Machine Learning Model

* **Random Forest Regressor**
* Inputs:

  * Slope
  * Vegetation density
  * Soil moisture
  * Distance to roads
* Output:

  * Predicted wildfire resistance value

---

## 🧭 Corridor Mapping

* Uses **least-cost path analysis** (Dijkstra algorithm)
* Identifies optimal wildfire spread pathways
* Generates a binary corridor map

---

## 📊 Outputs

* Wildfire resistance surface map
* Wildfire corridor map
* Environmental layer visualizations
* `wildfire_corridor_results.xlsx`

---

## ⚙️ Requirements

Install dependencies:

```bash
pip install numpy pandas matplotlib scikit-learn scipy openpyxl
```

---

## 🚀 How to Run

```bash
python wildfire_corridor_mapping.py
```

---

## 🌍 Applications

* Wildfire risk assessment
* Fire management planning
* Landscape connectivity analysis
* Disaster preparedness
* Climate change impact studies

---

## 🔬 Future Improvements

* Integrate real satellite data (Sentinel-2, MODIS)
* Include wind and temperature dynamics
* Use cellular automata for fire spread simulation
* Apply graph optimization for large-scale landscapes
* Incorporate time-series wildfire modeling


