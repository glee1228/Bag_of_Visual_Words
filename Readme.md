# Bag of Visual Words Image Classifier
### : Visual Categorization with Bags of Keypoints

### [Paper](https://www.cs.cmu.edu/~efros/courses/LBMV07/Papers/csurka-eccv-04.pdf)

Implementation of a content based image classifier using the [bag of visual words model](https://en.wikipedia.org/wiki/Bag-of-words_model_in_computer_vision) in Python.


## Paper Result
![](https://github.com/glee1228/TIL_AI/blob/master/Image/Phow1.png)

## Our Result(best)
Weak Features, M = 2500, Single, Level 0 (1x1),Linear SVM(C=100.0)

### 31%

Strong Feature, M = 600, Single, Level 0 (1x1),Linear SVM(C=200.0 and 250.0)

### 40%

## Usage

Google Colab link : https://colab.research.google.com/drive/1_URYuLjPFqQGQ_-bWpwYIAV1NdV9rPl6

**Google Drive Link** for Download .pkl files


## Train & Test

**Click** Google Colab Link -> Runtime type change (GPU) -> Variable **run_all_process = True** -> Run all


## Process

```
1. Prepare Dataset : Caltech-101 Dataset

2. feature extraction : SIFT descriptors - Opencv Version(3.4.2.16) Downgrade for SIFT Features

3. clustering and build codebook : K-means clustering algorithm 

4. Image representation(making the histogram of features) : Vector Quantization 

5. classifier learning and recognition : SVM Classifier
```

## Referenced Code 

BoW Process:https://github.com/CyrusChiu/Image-recognition

K-Means Clustering using GPU : https://github.com/ilyaraz/pytorch_kmeans

Multi-class Linear SVM using GPU : https://github.com/murtazajafferji/svm-gpu


Porting by glee1228@naver.com
