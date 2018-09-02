# Convolutional Neural Networks for Sentence Classification

This repository contains the code which was used for the paper **Sentiment Analysis of E-Commerce Reviews with Convolutional Neural Network using Natural Language Processing** by Rohan Sawant. It started out as fork of [Alexander Rakhlin's Convolutional Neural Networks for Sentence Classification in Keras ](https://github.com/alexander-rakhlin/CNN-for-Sentence-Classification-in-Keras).

### Dataset
The dateset used for in this repo could be found on  [Kaggle](https://www.kaggle.com/nicapotato/womens-ecommerce-clothing-reviews).

## Code

### 1. Training the Model
To train a new model set ... in [sentiment_cnn.py](https://github.com/CT83/Womens-Ecommerce-Clothing-Reviews-CNN-for-Sentence-Classification-in-Keras/blob/master/sentiment_cnn.py)

`model_load = False`

`grid_search = False`


### 3. Evaluating the Model
To run the model on test set ... in [sentiment_cnn.py](https://github.com/CT83/Womens-Ecommerce-Clothing-Reviews-CNN-for-Sentence-Classification-in-Keras/blob/master/sentiment_cnn.py)


`model_load = True`

`grid_search = False`


### 2. Running Grid Search
To run grid search update the **grid params** in [sentiment_cnn.py](https://github.com/CT83/Womens-Ecommerce-Clothing-Reviews-CNN-for-Sentence-Classification-in-Keras/blob/master/sentiment_cnn.py) and set

`model_load = False`

`grid_search = True`

**also**

`batch_size = [10]`

`epochs = [10, 15, 20, 25, 30, 35]`

`optimizer = ['Adamax']`


## Conclusion
The model [CNN-Adamax-Final](https://github.com/CT83/Womens-Ecommerce-Clothing-Reviews-CNN-for-Sentence-Classification-in-Keras/blob/master/CNN-Adamax-Final) was trained with **25 Epochs**, **10 Batch Size**, **Adamax Optimizer** and **4 Convolutional Layers**. This is where the paper diverged from the material which inspired it. The deeper neural network allowed it to better fit to the data.