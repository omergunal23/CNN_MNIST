# CNN_MNIST
ELE489-Fundamentals of Machine Learning HW4

This project implements various CNN architectures on MNIST dataset.
(MNIST dataset contains numbers from 0 to 9 with 28x28 grayscaled images, 60000 total samples)
- Baseline CNN model is implemented.
- 3 different architectural types is implemented and effect of them are observed by comparing with baseline CNN model.
- Hyperparameter optimiztion is done to get the best model.
- Some parameters are observed which breaks the CNN model to yield poor accuracy results.

CNN_MNIST.ipynb
1) Necessary libraries are imported.
2) Dataset is splitted as train-test.
3) Distributions of the output numbers are observed.
4) Baseline CNN model: Conv→ ReLU → MaxPool → Conv → ReLU → MaxPool → Flatten → Dense → ReLU → Dropout(0.5) → Dense(10) → Softmax is implemented.
5) Tested with test dataset.
6) 3 different architectural types is implemented, every change on compared to the baseline CNN model is commented on the code:
  • Deeper network 
  • Different kernel sizes (1×1, 5×5)
  • Different activation functions (LeakyReLU, Tanh)
  • Add BatchNorm, GlobalAveragePooling, or skip connections
7) Hyperparameter optimization is done by changing:
  • Learning rate
  • Optimizer (Adam vs SGD)
  • Batch size
  • Dropout rate
  • Weight initialization
8) 3 failed experiments are done intentionally to degrade the performance and effects of them are observed.
