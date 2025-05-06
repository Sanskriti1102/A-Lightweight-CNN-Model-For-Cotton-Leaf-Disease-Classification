
# 🌿 A Lightweight CNN Model for Cotton Leaf Disease Classification

## 🧠 Overview
This project implements a lightweight Convolutional Neural Network (CNN) for classifying cotton leaf diseases. The model is designed to be computationally efficient and suitable for deployment on edge devices, providing real-time disease detection to assist farmers in timely intervention.

## 🎯 Objectives
- Develop a custom CNN model that balances performance and computational cost.
- Accurately classify cotton leaves into four categories.
- Enable real-time, on-field usage by making the model lightweight.

## 📂 Dataset
The dataset used in this project includes images categorized into the following four classes:
- **Healthy**
- **Alternaria Leaf Spot**
- **Bacterial Blight**
- **Curl Virus**

All images are resized to **256×256×3** before being fed into the model.

## 🏗️ Model Architecture
The proposed CNN model includes:
- **Input Layer**: Accepts 256×256×3 images.
- **3 Convolutional Layers**: Each followed by Batch Normalization, ReLU activation, and Max Pooling.
- **Flatten Layer**: To convert 2D matrices into a 1D vector.
- **Fully Connected Layers**: Two dense layers for feature learning.
- **Output Layer**: Softmax activation to classify into 4 classes.

### 🔧 Layer-wise Details:
| Layer Type         | Parameters                         |
|--------------------|-------------------------------------|
| Convolutional      | 3×3 filters, stride 1               |
| Batch Normalization| Applied after each conv layer       |
| Activation         | ReLU                                |
| Max Pooling        | 2×2 window                          |
| Dense (FC Layers)  | 128 and 64 units                    |
| Output Layer       | 4 units with Softmax activation     |

## 🧪 Performance
- **Accuracy Achieved**: ~97.3%
- **Model Size**: Small enough for edge deployment.
- **Inference Time**: Optimized for real-time use.

## 🔍 Evaluation
- **Confusion Matrix** and **classification report** were used for performance analysis.
- The model was tested on unseen data to ensure generalization.

## 🛠️ Tools & Technologies
- Python
- TensorFlow / Keras
- NumPy, Pandas, Matplotlib
- Google Colab / Jupyter Notebooks

## 🚀 Future Work
- Integrate with a mobile app for on-field diagnosis.
- Expand dataset with regional varieties and more disease types.
- Incorporate explainable AI techniques to interpret predictions.

## 📌 Conclusion
This lightweight CNN offers an effective and deployable solution for real-time classification of cotton leaf diseases, helping farmers take timely actions and reduce crop losses.

