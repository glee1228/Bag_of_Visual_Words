# Bag of Visual Words Image Classifier

Implementation of a content based image classifier using the [bag of visual words model](https://en.wikipedia.org/wiki/Bag-of-words_model_in_computer_vision) in Python.

colab link : https://colab.research.google.com/drive/1_URYuLjPFqQGQ_-bWpwYIAV1NdV9rPl6

**Google Drive Link**

for Download .pkl files

**Prepare Cigar-10 Dataset**

using keras.datasets load functions

**Opencv Downgrade** 

3.4.3 version can not be used because of patents on SIFT

**Bag of Features Process** 

1. feature extraction : SIFT descriptors 

2. clustering and build codebook : k-means algorithm 

3. Image representation(making the histogram of features) : Vector Quantization 

4. classifier learning and recognition : SVM Classifier