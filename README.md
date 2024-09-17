# Building-a-Neural-Network-from-Scratch 🧠
Semester 05-Deep Neural Networks module assigment 01

## Objectives 🎯

- Construct that neural network according to the given problem. (CS3630 Assignment 1.pdf) 
- Implement the back-propagation algorithm, and use gradient descent to train the network. 
- Use cross-entropy cost function on a Softmax function for training. 
- All but the last fully connected layers have ReLU as the activation function.
- For given weight&bias sets, Calculate the gradients using the back propagation implementaton.
- Study the effect of learning rate.


## Neural Network implementation with Forward and Backward propagation

### Back Propagation
- Derivative of the Cross Entropy Loss

     \[ \delta = \hat{y} - y_{\text{true}} \]

- Gradient of the error for hidden layers with respect to weighted input

     \[ \delta_i = \delta_{i+1} \cdot W_{i+1}^T \cdot \text{ReLU}'(z_i) \]

- Gradient of the weights

     \[ \frac{\partial L}{\partial W_i} = \frac{1}{m} \cdot \delta_i \cdot a_{i-1}^T \]

- Gradient of the biases

     \[ \frac{\partial L}{\partial b_i} = \frac{1}{m} \cdot \sum_{j=1}^{m} \delta_i^{(j)} \]
<!-- ## Creating a Virtual Environment
### On macOS

```
cd /path/to/your/project
python3 -m venv env
source env/bin/activate
```

### On Windows
```
cd \path\to\your\project
python -m venv env
env\Scripts\activate
```

## Dpendencies

pip install pandas
pip install numpy -->