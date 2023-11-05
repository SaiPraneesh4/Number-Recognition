# Number-Recognition
This code is a Python script for building, training, and saving a neural network model for digit recognition using the Keras library. Here's a description of each section of the code:

1. Importing Libraries:
   - `numpy` is imported for numerical operations.
   - `mnist` is imported from `keras.datasets` to load the MNIST dataset.
   - Various components from Keras are imported for building and training the neural network model.

2. Loading the MNIST Dataset:
   - The MNIST dataset, consisting of handwritten digit images and their labels, is loaded into `X_train`, `y_train`, `X_test`, and `y_test` arrays.

3. Preprocessing the Data:
   - The images are reshaped to have a 28x28 size and a single channel (grayscale).
   - The pixel values are normalized to be between 0 and 1.
   - Labels are one-hot encoded to be suitable for training.

4. Building the Neural Network Model:
   - A sequential model is created using Keras.
   - The model consists of a flattening layer followed by two dense (fully connected) hidden layers with ReLU activation functions, and an output layer with a softmax activation function for digit classification.

5. Compiling the Model:
   - The model is compiled with the categorical cross-entropy loss function, the Adam optimizer, and accuracy as the evaluation metric.

6. Training the Model:
   - The model is trained using the training data for 10 epochs with a batch size of 200. The training progress is printed with verbosity level 2.
   
7. Saving the Model:
   - The trained model is saved as 'digit_recognition_model.keras' for later use.

8. Loading the Model and Making Predictions:
   - The code provides an example of how to load the saved model and make predictions on new scanned images.
   - The loaded model and an example scanned image ('download.jpeg') are used.
   - The scanned image is preprocessed similarly to the training data.
   - The model makes a prediction on the scanned image, and the predicted digit is printed.

This code is a digit recognition using a simple feedforward neural network with Keras. It can serve as a starting point for building more complex digit recognition models or for implementing other image classification tasks.
