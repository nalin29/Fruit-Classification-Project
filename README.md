# Fruit-Classification-Project
Exploration into CNN classification using the Keras API and fruit-360 dataset from Kaggle
In this project using the Tensorflow Keras API I create a series of CNN models and evaluate the best one on the Fruit-360 dataset from Kaggle which contains 131 fruits and vegetables to classify.

Ultimately the best model was a transfer learning model based on pretrained weights from ResNet50
Link to model Files: <url>https://drive.google.com/file/d/1NQjai2o9rIqRwpoV6iCJ8sOamJs0_K1e/view?usp=sharing</url>

## Custom CNN Model
This model has 4 convolutional layers and 2 fully connected layers. The fully connected layers implement dropout as a method of regularization.

### Confusion Matrix as well as score on dataset:

![Alt text](Images/confusion_matrix1.png?raw=true "Confusion Matrix Transfer Model: ")


### Loss and Accuracy Per Epoch:

![Alt text](Images/plot_data1.png?raw=true "Loss and Accuracy Graphs: ")

### Test Image Batch:

![Alt text](Images/test_images1.png?raw=true "Test Images: ")

Green means Passed, Red for Fail

## Transfer Learning
Transfer Learning is done on ResNet50 pretrained on Imagenet.
The features computed by ResNet is average pooled and passed into two fully connected layer where softmax layer outputs predictions.


### Confusion Matrix as well as score on dataset:

![Alt text](Images/confusion_matrix2.png?raw=true "Confusion Matrix Transfer Model: ")


# Loss and Accuracy Per Epoch:

![Alt text](Images/data_plot.png2?raw=true "Loss and Accuracy Graphs: ")

# Test Image Batch:

![Alt text](Images/test_images.png2?raw=true "Test Images: ")

Green means Passed, Red for Fail