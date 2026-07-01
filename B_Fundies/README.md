# Fundies (a.k.a. Fundamentals)

This folder contains mini-projects that act as recipes for different use cases in deep learning. Everything is implemented using the [PyTorch](https://github.com/pytorch/pytorch) library.


## Projects so far
1. [Irrigation prediction pipeline](01_irrigation_need/): basic feed-forward network trained on a tabular dataset containing both numerical and categorical features. Tricks used include adjusting class weights and kaiming initialization.
2. [Electricity consumption prediction](02_electricity_consumption/): time-series problem where we attempt to predict future electricity consumption for 300+ clients. Different sequential prediction models (LSTM, GRU, Exponential Smoothing, Prophet, N-BEATS, LightGBM, Ensemble of LightGBM, Toto) are built and contrasted against classic models (ARIMA, Holts-Winter).
<!-- https://www.sciencedirect.com/org/science/article/pii/S1546221825008872 -->
<!-- https://www.sciencedirect.com/science/article/pii/S0169207021001874 -->


## Technical details

### Python version
3.12.8

### Libraries used
- pandas
- numpy
- scikit-learn
- torch
- tqdm