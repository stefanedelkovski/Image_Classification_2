## CNN Image Quality Classifier

### Overview

The first approach, although it was functional, was a cheesy approach. So I decided to
take a step forward and build a DNN. This is a Keras model trained on GPU in **Google Colab**. 
It is a simple convolutional neural network architecture consisting of two convolutional layers and
pooling layers, flatten, a fully connected and output layer. The model generalizes
well in few epochs.

### Usage

The usage is straightforward - run the script in Google Colab (*runtime=GPU*). The only requirement is 
to upload the **frames** folder and **scores.txt** to drive. The **.ipynb** file does the following:

1. Connect to your drive

2. Generate the necessary requirements.txt file

3. Generate a training script with .py extension

4. Generate a predicting script with .py extension

5. *Quietly* install the requirements

6. Load images, train the model, save the model

7. Few prediction examples on the train and validation data 
   via terminal with an image as an argument


### Additional info
The model has ~31 mil. trainable parameters, which makes the model unfeasible for CPU.
Google Colab stores files only during runtime, which is the reason why I use **Drive** for
loading the data. 