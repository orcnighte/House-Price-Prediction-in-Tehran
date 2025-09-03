# House Price Prediction - District 4 Tehran

This project implements a neural network model to predict house prices in District 4 of Tehran.  

### Model Architecture
- 4 layers fully connected  
- 53 neurons in total  
- Activation functions: ReLU for hidden layers, linear for output  

### Dataset
- 24 features (e.g., area, number of rooms, location, age of building, etc.)  
- All features are scaled using MinMaxScaler for stable and efficient training  

### Training Process
1. Initial training with SGD  
   - Train and Validation sets separated  
   - Checked R² scores and confirmed no overfitting  

2. Final training with Mini-Batch GD  
   - Combined Train + Validation to maximize training data  
   - Batch size: 16  
   - Number of epochs: adjustable (default 50)  
   - Result: R² > 0.99 on both Train and Validation  

### Features

- Predicts house prices using 24 features  
- 4-layer neural network with 53 neurons  
- Normalized features with MinMaxScaler  
- Mini-Batch GD with batch size = 16  
- Evaluates performance using R² Score  
- Adjustable learning rate, batch size, and epochs  

### Installation

1. Clone the repository:
```bash
git clone https://github.com/orcnighte/House-Price-Prediction-in-Tehran
.git
