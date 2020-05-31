## Project Overview
In this Project, I trained a Convolutional neural network to recognize features in an image where the subject can be anywhere in the image. I did this by building a horses-or-humans classifier that will tell us if a given image contains a horse or a human, where the network is trained to recognize features that determine which is which.

## Dependencies
* Google Colab
* TensorFlow
* Python

## Data Processing
Let's set up data generators that will read pictures in our source folders, convert them to float32 tensors, and feed them (with their labels) to our network. We'll have one generator for the training images and one for the validation images. Our generators will yield batches of images of size 300x300 and their labels (binary). Finally, we will preprocess our images by normalizing the pixel values to be in the [0, 1] range (originally all values are in the [0, 255] range).

## Building Model
* Imported tensorflow
* Initialised a neural network sequence
* Added convolutional layers and then flatten the final result to be feed into the densely connected layers.

## Training
Let's train for 15 epochs. The Loss and Accuracy are a great indication of progress of training. It's making a guess as to the classification of the training data, and then measuring it against the known label, calculating the result. Accuracy is the portion of correct guesses.

## Running the model
Let's now take a look at actually running a prediction using the model. The code in the notebook will allow you to choose 1 or more files from your file system, it will then upload them, and run them through the model, giving an indication of whether the object is a horse or a human. You can download images from the internet to your file system to try them out!


## Visualization

