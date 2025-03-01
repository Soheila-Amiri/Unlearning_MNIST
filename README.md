# Project summary
This work explores unlearning class '6' from the MNIST dataset by replacing it with class '3'.<br>
The weights most responsible for predicting '6' are identified, while others are frozen. The model is fine-tuned with a custom loss function that favors class '3' while penalizing class '6'.<br>
A modified ResNet-50 model, adjusted for MNIST with a custom first convolutional layer to reduce downsampling, is used.<br>
The model is then fine-tuned on a retain dataset (excluding class '6') to improve performance.
