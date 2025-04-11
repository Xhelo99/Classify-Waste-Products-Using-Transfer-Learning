# 🧠 Classify Waste Products Using Transfer Learning & Fine-Tuning

This project applies **Transfer Learning and Fine-Tuning** to classify different types of waste products in organic and recyclable using deep learning and convolutional neural networks (CNNs). The goal is to automate waste sorting for improved recycling efficiency and environmental impact.

## 🚀 Key Features

- Uses **Transfer Learning** with `VGG16` as the base model
- Implements **Fine-Tuning** to improve model performance
- Achieves over **90% accuracy** on validation data
- Saves the best performing model using `Model Checkpoint`

## 🧰 Tech Stack

- Python 🐍
- TensorFlow / Keras
- NumPy
- Matplotlib
- Scikit-learn
- OpenCV (optional for image handling)

## 📊 Dataset

The dataset used is the

o-vs-r-split/
└── train
    ├── O
    └── R
└── test
    ├── O
    └── R

## 🏗️ How It Works

1. **Load and preprocess images** using `ImageDataGenerator`
2. **Use a pre-trained CNN** (VGG16) without the top layer
3. **Freeze base layers** and add custom dense layers for classification
4. Train the model with early stopping and learning rate scheduling
5. **Unfreeze some base layers** and continue training (fine-tuning)
6. Save the best model to disk

## 📈 Model Performance

- Validation Accuracy: ~92%
- The model generalizes well due to augmentation and fine-tuning
- Confusion matrix and classification report help analyze errors

