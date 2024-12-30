# 🐶 End-to-End Multiclass Dog Breed Classification 🐶

This repository demonstrates how to build an end-to-end multiclass image classifier using TensorFlow 2.0 and TensorFlow Hub to identify dog breeds from images.

## Problem
Identify the breed of a dog in a given image. For example, determine the breed of a dog that joins you during dinner.

## Data
Dataset: [Kaggle Dog Breed Identification](https://www.kaggle.com/c/dog-breed-identification)

## Evaluation
Predict probabilities for each dog breed for test images.  
Details: [Kaggle Evaluation](https://www.kaggle.com/c/dog-breed-identification/overview/evaluation)

## 4. Features
- The task involves **images** (unstructured data), making deep learning/transfer learning suitable.
- There are **120 dog breeds** (classes).
- The **training set** contains over **10,000 labeled images**.
- The **test set** also contains over **10,000 unlabeled images**, requiring predictions.
 

---

## Key Steps in the Notebook
1. **Mounting Google Drive**: The notebook starts by mounting Google Drive to access the dataset.
2. **Unzipping the Dataset**: Extracting the dataset to retrieve images and labels.
3. **Environment Setup**: Importing necessary libraries like TensorFlow and TensorFlow Hub.
4. **Data Preparation**:
   - Loading and exploring the labels.
   - Converting images and labels into Tensors (numerical representations).
   - Ensuring the number of filenames matches the number of images.
5. **Data Visualization**: Displaying sample images and label distributions.
6. **Label Encoding**: Converting breed labels into boolean arrays for model training.
7. **Model Building**: Usingfrom TensorFlow and TensorFlow Hub to build and train the model.
8. **Evaluation and Prediction**: Evaluating the model on the test set and making predictions.

---

### Solution

I used a deep learning pretrained model named **MobileNetV2** for this project. This has been one of the best visualizing projects I’ve ever done. After training with 3k images from the entire dataset of 10k images, I achieved an accuracy of **80%**.

---

## Key Functions Used:
1. **`os.listdir()`**: 
   - Used to access all the files in a folder in string format.

2. **`to_numpy()`**: 
   - Converts a DataFrame column to a list of numpy arrays.

3. **Label Encoding**: 
   - I turned each label into a boolean array for model training.

4. **`numpy.argmax()`**: 
   - Used to find the index of the maximum value in an array.

---

This approach enabled effective image classification using deep learning, and I was able to visualize the results with great clarity.

