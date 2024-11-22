
# Marabou Implementation

This is a submission by Gatum Erlangga for Neural Network Verification class

## Requirements
The code is run on ```python==3.10```, with ```conda``` environment. To create ```conda``` environment, run the following command:
```
conda create -n marabou python==3.10
```
After that, install the following libraries.
```
numpy==1.26.4
tensorflow==2.12.0
onnx==1.17.0
onnxruntime==1.19.2
tf2onnx==1.16.1
scikit-learn==1.5.2
maraboupy==2.0.0 (latest)
```

## Code Implementations
There are two implementations using two different dataset and simple classification model, such as iris and fashion_mnist dataset. The implementations located in ```/fashion_mnist``` and ```iris``` for fashion_mnist and iris dataset respectively. The description of each file are described as follows: \
```/iris/marabou_verification.ipynb```: This file contains code implementation of neural network verification using marabou \
```/iris/model.ipynb```: Implement model training on the corresponding dataset (iris) using tensorflow. \
```*.onnx```: Exported model in onnx format \
```/iris/iris_binary_classification_model_tf```: Exported model from tensorflow

## Problem
In the implementation of fashion_mnist, the SAT and UNSAT solution were not found. This may due to the input size which is 28 x 28, make it too big. Meanwhile, the implementation of iris dataset is successfully done, taking advantage of its size.
 
## Author
- [@erlanggagatum](https://www.github.com/erlanggagatum)