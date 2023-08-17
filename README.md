# DeepECG: ECG Classification using Machine Learning and Deep Learning Methods

This repository contains programs for ECG classification based on Machine Learning (ML) and Deep Learning (DL) methods. The repository includes two datasets:

1. The `training2017.zip` file contains single-electrode voltage measurements taken as the difference between RA and LA electrodes with no ground. This data is sourced from The 2017 PhysioNet/CinC Challenge.

2. The `MIT-BH.zip` file contains two electrode voltage measurements: MLII and V5.

## Prerequisites

- Python 3.5 and higher
- Keras framework with TensorFlow backend
- Numpy, Scipy, Pandas libraries
- Scikit-learn framework

## Running the Program

Follow these steps to run the program:

1. Extract the contents of the `training2017.zip` and `MIT-BH.zip` files into the `training2017/` and `MIT-BH/` folders, respectively.

2. If you want to use the 2D Convolutional Neural Network for ECG classification, execute the `CNN_ECG.py` file with the following commands:

   - To train your model on the 2017 PhysioNet/CinC Challenge dataset:
     ```
     python CNN_ECG.py cinc
     ```
   - To train your model on the MIT-BH dataset:
     ```
     python CNN_ECG.py mit
     ```

3. If you want to use the 1D Convolutional Neural Network for ECG classification, run the `Conv1D_ECG.py` file with the following command:
