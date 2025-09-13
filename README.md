# 🏠 House Price Prediction - District 4, Tehran

## Project Overview
Predict house prices in **District 4 of Tehran** using a **Neural Network**.  

The model uses **24 input features** (e.g., area, number of rooms, location, building age) and outputs the predicted price.  

- **Training Methods:**  
  - Batch Gradient Descent → R² ≈ 0.82  
  - Mini-Batch Gradient Descent → R² ≈ 0.81  
- **Objective:** Maximize R² on unseen test data.

---

## Model Architecture (Graphical)

```text
         ┌─────────────┐
         │ Input Layer │ 24 features
         └─────┬───────┘
               │
        ┌──────▼──────┐
        │ Hidden L1   │ 16 neurons, ReLU
        └──────┬──────┘
               │
        ┌──────▼──────┐
        │ Hidden L2   │ 8 neurons, ReLU
        └──────┬──────┘
               │
        ┌──────▼──────┐
        │ Hidden L3   │ 4 neurons, ReLU
        └──────┬──────┘
               │
         ┌─────▼─────┐
         │ Output L   │ 1 neuron, Linear
         └───────────┘


### Installation

1. Clone the repository:
```bash
git clone https://github.com/orcnighte/House-Price-Prediction-in-Tehran
.git
