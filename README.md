# Digit Recognition Using Convolutional Neural Networks (CNN)

## This Project was Implemented using the following :
  * Keras for Creating and Implementing the CNN Model
  * NumPy for Data Pre Processing
  * PIL for GUI
  * OpenCV for Drawing in GUI
  * MNIST Dataset for Numbers [0 .. 9]
 
## Implementation of the Model 
  * The Model was Implemented by using a Constructing a Basic CNN using Keras Framework.
  * First the Data is Imported from MNIST Dataset, Reshaped its Dimentions, Normalized.
  * Then a Sequential Model is Built using Keras Framework in the Following Sequence :
    * Conv2D_1Layer - > MaxPooling_1Layer - > Conv2D_2Layer - > MaxPooling2Layer -> Dropout -> Flatten the O/P -> Dense_ANN -> SoftMax_Layer.
  * The Constructed Model is Trained in Mini Batches for 10 for Learning 10 Classes.
  * Saves the Constructed Model to local disk as "digit_recog_cnn_model.h5".
  * In Another Python File "load_n_draw.py", it loads the trained "digit_recog_cnn_model.h5" and uses PIL & OpenCV to make GUI.

## How to Run ?
  1. First Train and Save the Model by Running "digit_recognition_cnn.py"
  2. Then Run "load_n_draw.py" to load the Trained Model and Predict the outcome based on your Input on GUI.
