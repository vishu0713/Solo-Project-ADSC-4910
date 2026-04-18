# Facial Emotion Detection using CNN (PyTorch)

## 📌 Project Overview

This project builds a deep learning model to detect human emotions from facial images using a Convolutional Neural Network (CNN) implemented in PyTorch. The model is trained on the FER2013 dataset and classifies images into seven different emotions.

---

## 🎯 Objectives

* Apply deep learning techniques on image data
* Build and train a CNN using PyTorch
* Evaluate model performance using accuracy and confusion matrix
* Interpret results and identify limitations

---

## 📊 Dataset

The project uses the **FER2013 dataset**, a widely used benchmark for facial emotion recognition.

### Dataset Details:

* Image size: 48 × 48 pixels
* Grayscale facial images
* ~35,000 samples
* 7 emotion classes:

  * Angry (0)
  * Disgust (1)
  * Fear (2)
  * Happy (3)
  * Sad (4)
  * Surprise (5)
  * Neutral (6)

Although stored in CSV format, each row represents pixel values of an image. These are converted into image format during preprocessing, making this an **unstructured image-based project**.

---

## 🧠 Model Architecture

A Convolutional Neural Network (CNN) is used because it is effective for image classification tasks.

### Model Components:

* Convolutional Layers (feature extraction)
* ReLU Activation
* Batch Normalization
* Max Pooling
* Fully Connected Layers
* Dropout (to reduce overfitting)

---

## ⚙️ Installation & Setup

### 1. Clone the repository

```bash
git clone <your-repo-link>
cd facial-emotion-detection
```

### 2. Create virtual environment (optional)

```bash
python -m venv venv
venv\Scripts\activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

---

## ▶️ How to Run the Project

1. Open Jupyter Notebook:

```bash
jupyter notebook
```

2. Open the file:

```
Solo_Project.ipynb
```

3. Run all cells from top to bottom.

---

## 🔄 Project Workflow

1. Load dataset
2. Convert pixel values into images
3. Normalize data
4. Train-test split
5. Build CNN model
6. Train model
7. Evaluate performance
8. Visualize results

---

## 📈 Results

* **Test Accuracy:** ~58%

### Interpretation:

The model performs well on clear emotions such as **Happy** and **Surprise**, but struggles with similar emotions like **Sad**, **Fear**, and **Neutral**.

This is expected because:

* The dataset is low-resolution (48×48)
* Some emotions have very subtle differences

---

## 📊 Evaluation Metrics

* Accuracy
* Confusion Matrix

---

## 🧠 Key Learnings

* CNNs are effective for image-based tasks
* Data preprocessing significantly impacts performance
* Emotion recognition is challenging due to subtle facial differences

---

## ⚠️ Limitations

* Low-resolution dataset
* Class overlap (similar emotions)
* Moderate accuracy

---

## 🚀 Future Improvements

* Use deeper models (ResNet, VGG)
* Apply data augmentation
* Hyperparameter tuning
* Use higher-quality datasets

---

## 📦 Dependencies

* torch
* torchvision
* numpy
* pandas
* matplotlib
* scikit-learn
* seaborn

---

## 🔑 API Keys

No API keys are required for this project.

---

## 👨‍💻 Author

Vishvam Sanghadiya

---

## 📌 Conclusion

This project demonstrates how deep learning can be applied to facial emotion detection. Despite dataset challenges, the CNN model successfully learns meaningful patterns and achieves reasonable performance.
