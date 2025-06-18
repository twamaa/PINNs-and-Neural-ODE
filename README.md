# EA Assignment 3 - PINNs and Neural ODEs

**Full Name:** Twamaa Makame  
**Assignment Title:** EA Assignment 3  
**Roll Number:** Z6003  


## Description

This repository contains solutions for EA Assignment 3 which focuses on:  
1. Estimating cardiac activation times on a 2D domain using sparse data.  
2. Comparing traditional feedforward neural networks with Physics-Informed Neural Networks (PINNs).  
3. Using Neural Ordinary Differential Equations (Neural ODEs) for binary classification on a 2D dataset.  

The code is organized into sections that generate synthetic data, define conduction velocity, train data-only and PINN models, visualize results, and build Neural ODE classifiers.

##  Repository Structure

/EA_Assignment3/  
│  
├── README.md               <- This file  
├── requirements.txt        <- Dependencies for the project  
│  
├── /src/                   <- Python scripts and notebooks  
│   ├── pinn_model.py  
│   ├── ode_model.py  
│   ├── data_generation.py  
│   └── visualization.py  
│  
└── /test/                  <- Optional test cases and outputs  
    └── sample_inputs_outputs/

## 🚀 How to Run

1. Clone the repository:
   git clone[(https://github.com/twamaa/PINNs-and-Neural-ODE)]

2. Install dependencies:
   pip install -r requirements.txt

3. Open the Jupyter notebooks in the `/src/` folder or run scripts directly for:
   - Generating synthetic data  
   - Training and evaluating both models  
   - Producing visualizations

## Dependencies

See `requirements.txt`. Key packages include:  
- numpy  
- matplotlib  
- torch  
- torchdiffeq  
- scikit-learn  
- pyDOE

##  Known Issues

- The PINN model occasionally produces high RMSE if the sparse points do not sample critical wavefront boundaries.  
- Neural ODE training can be slower than standard networks.

##  Assumptions

- Activation function and velocity maps are synthetic and idealized.  
- Moons dataset used for Neural ODE comparison is noise-injected but simplified.
