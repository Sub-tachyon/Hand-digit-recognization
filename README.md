# Hand-digit-recognization

This project demonstrates a simple handwritten digit recognition system using a neural network. It utilizes the popular MNIST dataset, which contains a large collection of handwritten digits.

The components used in my project are :

Libraries:

OpenCV (cv2)
NumPy (np)
Matplotlib (plt)
TensorFlow (tf)

MNIST Dataset:
  Loaded using tf.keras.datasets.mnist.
  
Data Preprocessing:
  Normalization using tf.keras.utils.normalize.
  
Neural Network Architecture:
   Sequential model with layers:
      Flatten layer
      Dense layers (with ReLU activation)
      Output Dense layer (with softmax activation)
      
Model Compilation:
   Using model.compile with 'adam' optimizer and 'sparse_categorical_crossentropy' loss.

Model Training:
   Using model.fit with training data and specified number of epochs.

Model Saving:
   Saved using model.save.

Custom Image Testing:
   Looping through custom images using os.path.isfile.
   Reading and preprocessing images using OpenCV. 
   Making predictions using the trained model.
   Displaying images and predictions using Matplotlib.
