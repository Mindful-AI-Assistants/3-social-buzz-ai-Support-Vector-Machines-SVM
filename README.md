
<br>
 
 
 \[[🇧🇷 Português](README.pt_BR.md)\] \[**[🇺🇸 English](README.md)**\]


<br>

# <p align="center">  Social [Buzz AI]() - Support Vector Machines (SVM)

<br><br>


<p align="center">
   <img src="https://github.com/user-attachments/assets/791a69e2-d09a-429f-9257-f6667fff5c04 ">
 </p>

<br><br>

[**Course:**]() Humanistic AI & Data Science (4th Semester)  
[**Institution:**]() PUC-SP  
**Professor:** [Erick Bacconi](https://www.linkedin.com/in/eric-bacconi-423137/)  



<br><br>


#### <p align="center"> [![Sponsor Mindful AI Assistants](https://img.shields.io/badge/Sponsor-%C2%B7%C2%B7%C2%B7%20Mindful%20AI%20Assistants%20%C2%B7%C2%B7%C2%B7-brightgreen?logo=GitHub)](https://github.com/sponsors/Mindful-AI-Assistants)


<!--Confidentiality Statement-->

<br><br>


> [!IMPORTANT]
>
> ⚠️ Heads Up 
>
> * Projects and deliverables may be made [publicly available]() whenever possible.
>
> * The course prioritizes [**hands-on practice**]() with real data in consulting scenarios.
>
> *  All activities comply with the [**academic and ethical guidelines of PUC-SP**]().
>
> * [**Confidential information**]() from this repository remains private in [private repositories]().
>
>

#  

<br><br><br>



> [!TIP]
>
> * [Access](https://github.com/Mindful-AI-Assistants/3-social-buzz-ai-Support-Vector-Machines-SVM/blob/cfd3ab9a47be09c8acd3dab569c39452d9f54593/Workbook/SVM.pdf): Workbook Support Vctor Machines (SVM)
> 
> * [Access](https://github.com/Mindful-AI-Assistants/3-social-buzz-ai-Support-Vector-Machines-SVM/blob/1567e7dbb69685b73403acb9e16b36d48b428315/Code_Support_Vector_Machines(SVM)/Code_Support_Vector_Machines_SVM.ipynb): 1- Code_SVM
>
> * [Access]():  2-Code_
>
>
> * [Access](https://github.com/Mindful-AI-Assistants/3-social-buzz-ai-Support-Vector-Machines-SVM/blob/d4f48fb3c1a922e2eba3a3faf6ce096643fc10f4/Dataset/Varejo.csv):  Dataset
>

 
<br><br>


<!--End-->


## Support Vector Machines (SVM)

Support Vector Machines (SVM) is a supervised machine learning algorithm for classification tasks. This repository provides a comprehensive explanation of SVM, including theory, concepts, comparative analysis, and illustrative plots.

<br>

## Applications

SVM is widely used in:

- Image recognition
- Text classification and natural language processing
- Bioinformatics
- Any binary classification problems requiring high accuracy and robustness

<br>


### Table of Contents

- [Overview](#overview)
- [Key Concepts](#key-concepts)
    - [Data Representation and Hyperplanes](#data-representation-and-hyperplanes)
    - [Support Vectors](#support-vectors)
    - [Soft Margin Classification](#soft-margin-classification)
    - [Non-linearly Separable Data and Kernel Trick](#non-linearly-separable-data-and-kernel-trick)
- [Algorithmic Details](#algorithmic-details)
- [Strengths and Weaknesses](#strengths-and-weaknesses)
- [Comparison with Other Classifiers](#comparison-with-other-classifiers)
- [Applications](#applications)
- [Illustrative Plots](#illustrative-plots)
- [References](#references)


<br><br><br>


# Support Vector Machines (SVM)

Support Vector Machines (SVM) is a supervised machine learning algorithm widely used for classification tasks. This repository contains a comprehensive explanation of the SVM algorithm, including its theory, mathematical foundations, key concepts, and practical considerations.


<br><br>

## Overview

Support Vector Machines classify data points by determining an optimal separator (hyperplane) that best distinguishes between different classes. The data points are mapped into an n-dimensional feature space, where $n$ is the number of features, and the classification is achieved by finding the hyperplane that maximizes the margin between classes.

<br><br>


## Key Concepts

### Data Representation and Hyperplanes

<br>

- Each data point is represented as a point in an n-dimensional space corresponding to its features.
- The SVM finds a hyperplane (line in 2D, plane in 3D, etc.) that separates classes with the widest possible margin.
- Support Vectors are the critical training examples closest to the hyperplane; they define the position and orientation of the optimal separating hyperplane.


<br>


### Support Vectors

<br>

- Support vectors are the most important training data points because they influence the position of the decision boundary.
- Other training points far from the boundary are ignored in the final model.

<br>

### Soft Margin Classification

<br>

- Introduces a slack variable to allow some misclassification to improve generalization.
- Soft margin allows some points to be on the wrong side of the margin but tries to classify the majority correctly.

<br>

### Non-linearly Separable Data and Kernel Trick

- When data cannot be separated by a linear hyperplane, SVM maps data into a higher-dimensional space where it becomes linearly separable.
- This is done via kernel functions that implicitly perform this mapping without explicitly computing coordinates in the high-dimensional space.
- Common kernels include Polynomial Kernel and Radial Basis Function (RBF).


<br><br>

## Algorithmic Details

<br>

- SVM optimization tries to maximize the margin between classes while minimizing classification errors.
- Different kernels allow SVM to handle linear and non-linear classification problems effectively.
- The choice of kernel and parameters significantly impacts the model performance.

<br><br>

## Strengths and Weaknesses of SVM

<br>

| Strengths | Weaknesses |
| :-- | :-- |
| High accuracy especially in high-dimensional spaces | Requires careful kernel selection |
| Memory efficient | Can overfit when features exceed samples |
| Fast classification process | Does not provide direct probability estimates |
|  | Not efficient with very large datasets |


<br><br>

## Applications

SVM is widely used in:

<br>

- Image recognition
- Text classification and natural language processing
- Bioinformatics
- Any binary classification problems requiring high accuracy and robustness


<br><br>


## Comparison of Common Machine Learning Algorithms (Part 1)

<br>

| Criterion | Decision Tree | Random Forest | Gradient Boosting (GBM) | Support Vector Machine (SVM) |
| :-- | :-- | :-- | :-- | :-- |
| Model Type | Single tree | Ensemble of trees (bagging) | Ensemble of trees (boosting) | Margin-based hyperplane classifier |
| Overfitting Tendency | High (if unpruned) | Lower (averaging many trees) | Moderate (can overfit if not tuned) | Possible if parameters poorly chosen |
| Interpretability | High | Moderate | Low | Difficult |
| Training Speed | Very fast | Reasonable | Slower than RF | Slow on very large datasets |
| Prediction Speed | Very fast | Fast | Moderate | Moderate |
| Scalability | Good | Good | Moderate | Poor on very large datasets |
| Normalization Needed | No | No | No | Yes |
| Non-linear Capability | Weak | Good | Very good | Excellent with kernel trick |
| Variable Importance | Easy to extract | Easy to extract | Easy to extract | Not native (requires permutation) |
| Typical Application | Simple interpretable models | Large-scale classification/regression | High performance competitions | Complex data, NLP, bioinformatics |


<br><br>

## Comparison of Common Machine Learning Algorithms (Part 2)

<br>


| Criterion | k-Nearest Neighbors (kNN) | Naive Bayes | Artificial Neural Networks (ANN) | XGBoost |
| :-- | :-- | :-- | :-- | :-- |
| Model Type | Instance-based (lazy) | Probabilistic | Deep learning | Gradient boosting ensemble |
| Overfitting Tendency | Low to moderate (data-dependent) | Moderate (assumes independence) | Can overfit without regularization | Moderate to low (with tuning) |
| Interpretability | Low | Moderate | Low | Low |
| Training Speed | Very fast (training = lazy) | Very fast | Slow | Moderate to slow |
| Prediction Speed | Slow (needs distance calc) | Very fast | Fast if hardware-accelerated | Fast |
| Scalability | Poor on big data | Good | Good (with hardware support) | Good |
| Normalization Needed | Yes | No | Yes | Yes |
| Non-linear Capability | Good | Weak (depends on distribution) | Excellent | Excellent |
| Variable Importance | No | No | No (opaque) | Yes |
| Typical Application | Small datasets, recommender | Text classification, spam filtering | Image, speech, NLP | Structured data competitions |


<br><br>


## Applications

### SVM is widely used in:

<br>

- Image recognition
- Text classification and natural language processing
- Bioinformatics
- Any binary classification problems requiring high accuracy and robustness


<br><br>

## Illustrative Plots

Below are essential Python code examples to generate plots illustrating SVM concepts. Run these scripts in a Jupyter notebook or Python IDE to visualize:

### 1. Linear SVM: Decision Boundary and Margin

<br>

```python
import numpy as np
import matplotlib.pyplot as plt
from sklearn import svm

X = np.array([[2, 3], [3, 3], [2, 4], [7, 8], [8, 8], [7, 9]])
y = [0, 0, 0, 1, 1, 1]

clf = svm.SVC(kernel='linear', C=1000)
clf.fit(X, y)

w = clf.coef_[^0]
b = clf.intercept_[^0]
x_plot = np.linspace(0, 10, 200)
y_plot = -(w[^0]/w[^1]) * x_plot - b/w[^1]

margin = 1/np.linalg.norm(w)
margin_up = y_plot + margin * np.sqrt(1 + (w[^0]/w[^1])**2)
margin_down = y_plot - margin * np.sqrt(1 + (w[^0]/w[^1])**2)

plt.scatter(X[:,0], X[:,1], c=y, s=100, cmap='coolwarm', edgecolors='k')
plt.plot(x_plot, y_plot, 'k-', label='Hyperplane')
plt.plot(x_plot, margin_up, 'k--', label='Margin')
plt.plot(x_plot, margin_down, 'k--')
plt.scatter(clf.support_vectors_[:,0], clf.support_vectors_[:,1], s=200,
            facecolors='none', edgecolors='k', label='Support Vectors')

plt.title('SVM Linear Kernel: Decision Boundary and Margin')
plt.xlabel('Feature 1')
plt.ylabel('Feature 2')
plt.legend()
plt.grid(True)
plt.show()
```

<br><br>

### 2. Soft Margin SVM: Overlapping Data

<br>

```python
import numpy as np
import matplotlib.pyplot as plt
from sklearn import svm

X_soft = np.array([[1, 2], [2, 2], [3, 3], [6, 5], [7, 8], [8, 8], [5, 5], [5, 6]])
y_soft = [0, 0, 0, 1, 1, 1, 0, 1]

clf_soft = svm.SVC(kernel='linear', C=1)
clf_soft.fit(X_soft, y_soft)

plt.scatter(X_soft[:,0], X_soft[:,1], c=y_soft, s=100, cmap='coolwarm', edgecolors='k')

w = clf_soft.coef_[^0]
b = clf_soft.intercept_[^0]
x_plot = np.linspace(0, 10, 200)
y_plot = -(w[^0]/w[^1]) * x_plot - b/w[^1]
plt.plot(x_plot, y_plot, 'k-', label='Hyperplane Soft Margin')
plt.scatter(clf_soft.support_vectors_[:,0], clf_soft.support_vectors_[:,1], s=200,
            facecolors='none', edgecolors='k', label='Support Vectors')

plt.title('Soft Margin SVM: Overlapping Data')
plt.xlabel('Feature 1')
plt.ylabel('Feature 2')
plt.legend()
plt.grid(True)
plt.show()
```


















<br><br>
<br><br>
<br><br>
<br><br>


## 💌 [Let the data flow... Ping Me !](mailto:fabicampanari@proton.me)


#### [Contact and Support]()

- For notebook files, detailed tutorials, or enhanced visualizations, please reach out.
- Interested in Python notebooks simulating these dynamics or advanced Humanistic AI models? Just ask!

<br>


#### <p align="center">  🛸๋ My Contacts [Hub](https://linktr.ee/fabianacampanari)


<br>

### <p align="center"> <img src="https://github.com/user-attachments/assets/517fc573-7607-4c5d-82a7-38383cc0537d" />



<br>



<p align="center">  ────────────── 🔭⋆ ──────────────


<p align="center"> ➣➢➤ <a href="#top">Back to Top </a>


<b><br>

#

##### <p align="center">Copyright 2025 Mindful-AI-Assistants. Code released under the  [MIT license.](https://github.com/Mindful-AI-Assistants/lacan-psychoanalysis-math-graphs/blob/28d9178584b831679dec129fb0aa040203ce0e9e/LICENSE.md)

