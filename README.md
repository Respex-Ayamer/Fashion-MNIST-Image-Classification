**Matunog-FlomereJoy_LW1_Image_Classification.ipynb**

Questions: (February 8, 2026)

1. What is the Fashion MNIST dataset?
The Fashion MNIST dataset is a collection of 70,000 grayscale images of clothing items such as shirts, shoes, bags, and coats, each sized 28×28 pixels. It is used as a standard benchmark dataset for training and testing machine learning and neural network models in image classification, as a more realistic replacement for the original MNIST handwritten digits dataset.

2. Why do we normalize image pixel values before training?
We normalize image pixel values to scale them from the range 0–255 down to 0–1 so that the neural network can train faster and more stably. Normalization helps prevent large gradient updates, improves numerical stability, and allows the optimizer to converge more efficiently.

3. List the layers used in the neural network and their functions.
The neural network typically uses:

- > Flatten layer - Converts the 28×28 image matrix into a one-dimensional vector so it can be processed by dense layers.
- > Dense (hidden) layer with ReLU activation - learns important features from the input and introduces non-linearity.
- > Dense (output) layer with Softmax activation - produces probability scores for each of the 10 clothing categories and selects the most likely class.

4. What does "epoch" mean in model training?
An epoch is one complete pass of the entire training dataset through the neural network during training. Each epoch allows the model to update its weights based on all training samples once.

5. Compare the predicted label and actual label for the first test image.
The predicted label is the class that the model thinks the image belongs to, while the actual label is the true class provided in the dataset. If both labels match, the prediction is correct; if they are different, the model has misclassified the image.

6. What could be done to improve the model’s accuracy?
The model’s accuracy can be improved by adding more hidden layers or neurons, increasing the number of training epochs, using a convolutional neural network (CNN) instead of a simple dense network, applying data augmentation, adjusting the learning rate, and using regularization techniques such as dropout.
