# Life-with-DL
Pet projects that make use of deep learning libraries in any way!

## Repo Structure
This repo contains a few sub-folders. See below.

### A_Hello_World
As the name of the folder suggests, it contains some straightforward "Hello World" projects.

- [Multiple classification on the iris dataset](A_Hello_World/iris.ipynb)
- [Multiple classification on the Fashion MNIST images dataset](A_Hello_World/Fashion_MNIST.ipynb)
  - Feed-forward Neural Network
  - Convolution + Pooling
  - Dropout + BatchNorm
  - Data Augmentation + Learning Rate Scheduling + Weight Decay
  - Fine-tune a Hugging Face Computer Vision Model (PyTorch)

### B_Fundies
This folder contains snippets for the fundamental types of deep learning projects (feedforward networks, sequential data, image-based applications, etc.).

- [Irrigation prediction pipeline](B_Fundies/01_irrigation_need/): basic feed-forward network trained on a tabular dataset containing both numerical and categorical features. Tricks used include adjusting class weights and kaiming initialization.
- [Electricity consumption prediction](B_Fundies/02_electricity_consumption/): time-series problem where we attempt to predict future electricity consumption for 300+ clients. Different sequential prediction models (LSTM, GRU, Exponential Smoothing, Prophet, N-BEATS, LightGBM, Ensemble of LightGBM, Toto) are built and contrasted against classic models (ARIMA, Holts-Winter).