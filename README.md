# deep-learning-architectures
MLP
Implementation: In this cell, we use the MNIST dataset to train a supervised learning model that classifies handwritten digits.
Source References  Scikit-Learn: Neural network models (supervised)
CNN
Convolutional Layer: Uses filters to scan the input and create a feature map.
Pooling Layer: Conducts dimensionality reduction to improve efficiency and limit the risk of overfitting.
(FC) Layer: Operates on flattened input to perform final classification based on extracted features.
Source TensorFlow: Convolutional Neural Network (CNN) Tutorial
RNN/LSTM
This model uses an RNN to perform sentiment analysis on the IMDB movie review dataset, generating a single output (positive/negative) from a sequence of text inputs.
Source TensorFlow Guide: Working with RNNs
1. Which architecture was most effective for its task?
The Convolutional Neural Network  is the superior architecture for images. As noted in the slides, CNNs use filters to identify patterns. By using Conv2D layers, the model can recognize an object  regardless of where they appear in the frame. This spatial hierarchy makes it good for computer vision.  The RNN is effective for text. Since reviews are sequences of words, the memory allows it to understand that "not good" is negative, whereas a standard MLP might just see the word "good" and misclassify it.
2. What challenges did you face during training or implementation?
One issue is vanishing gradients RNNs can forget the beginning of a long sentence. By using a LSTM (Long Short-Term Memory) the memory is preserved. Overfitting is another issue that leads to high training accuracy but poor test results.
3. How do you see these models being used in real-world applications?
An MLP could be used for credit scoring and fraud detection. These models are excellent for tabular data to predict if a transaction is legitimate. A CNN could identify pedestrians, stop signs, and lane boundaries for autonomous vehicles.  An RNN could be used as a translator  because these models understand the order of words, they are used to predict the next word in a text message or translate a sentence while maintaining the correct grammar.
