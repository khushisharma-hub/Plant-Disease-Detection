# 🌿 Plant Disease Detection Using CNN

**Domain**: Machine Learning & AI  
**Internship Program**: Tamizhan Skills Rise  
**Intern ID**: TS-RISE-MLAI-2514  
**Author**: Khushi Sharma  
**GitHub Repository**: [Plant Disease Detection](https://github.com/khushisharma-hub/Plant-Disease-Detection)  
**Demo Video**: [Watch Here](https://drive.google.com/file/d/1muKUOJeh_dSIEU-yRfIcshgeTR_8ndL8/view?usp=sharing)

---

## 📚 Table of Contents

1. [🔍 Project Overview](#-project-overview)  
2. [🎯 Objective](#-objective)  
3. [🛠️ Tools & Technologies](#️-tools--technologies)  
4. [📦 Dataset](#-dataset)  
5. [🔄 Workflow](#-workflow)  
6. [📊 Model Summary & Accuracy](#-model-summary--accuracy)  
7. [🖼️ Output Graph](#-output-graph)  
8. [🎥 Demo Video](#-demo-video)  
9. [✅ Conclusion](#-conclusion)  
10. [🔗 Important Links](#-important-links)

---

## 🔍 Project Overview

This project demonstrates the use of **Convolutional Neural Networks (CNN)** to detect plant diseases from leaf images. The goal is to help farmers identify diseases early through image analysis, aiding in agricultural decision-making and food security.

---

## 🎯 Objective

- Upload and preprocess plant leaf images  
- Train a CNN to classify diseases  
- Evaluate model performance with accuracy and loss graphs  
- Enable predictions from unseen data  
- Assist rural and agri-tech with a visual disease detection system

---

## 🛠️ Tools & Technologies

- **Python** (Google Colab)  
- **TensorFlow / Keras**  
- **Matplotlib, PIL**  
- **CNN (Convolutional Neural Networks)**  
- **ImageDataGenerator**  
- **Google Drive & GitHub** for storage

---

## 📦 Dataset

- 📁 **Classes**: `Healthy`, `Blight`, `Rust`, `Mildew`  
- 📦 **Download**: [plant_dataset.zip](https://github.com/khushisharma-hub/Plant-Disease-Detection/blob/main/plant_dataset%20(1).zip)  
- Images are already labeled and categorized into folders by class.

---

## 🔄 Workflow

1. 📤 Upload the ZIP dataset via Colab
2. 📂 Extract and clean corrupted images
3. 🧼 Normalize and augment image data
4. 🧠 Define CNN model architecture
5. 🎯 Train the model for 10 epochs
6. 📈 Plot training and validation accuracy
7. 🧪 Evaluate the final model

---

## 📊 Model Summary & Accuracy

| Layer (Type)       | Output Shape       | Parameters |
|--------------------|--------------------|------------|
| Conv2D             | (126, 126, 32)     | 896        |
| MaxPooling2D       | (63, 63, 32)       | 0          |
| Conv2D             | (61, 61, 64)       | 18,496     |
| MaxPooling2D       | (30, 30, 64)       | 0          |
| Flatten            | (25088)            | 0          |
| Dense (ReLU)       | (128)              | 3,211,392  |
| Dense (Softmax)    | (4)                | 516        |
| **Total Params**   |                    | **3.3M+**  |

- **Train Accuracy**: ~36%
- **Validation Accuracy**: ~27%
> Accuracy may improve with more data, fine-tuning, or model complexity.

---

## 🖼️ Output Graph

The model plots accuracy across epochs to visualize performance:

```python
plt.plot(history.history['accuracy'], label='Train')
plt.plot(history.history['val_accuracy'], label='Validation')
plt.title('Model Accuracy Over Epochs')
plt.xlabel('Epoch')
plt.ylabel('Accuracy')
plt.legend()
plt.grid(True)
plt.show()
🎥 Demo Video
📽️ Click to Watch Project Demo

✅ Conclusion
This project highlights the practical use of AI in agriculture, where CNN-based plant disease detection can assist farmers by automating the identification of leaf diseases. With further optimization and integration, it can be deployed as a mobile app for real-time diagnostics in rural areas.

🔗 Important Links
🔗 GitHub Repository: https://github.com/khushisharma-hub/Plant-Disease-Detection

📁 Dataset ZIP: Download Here

📘 Notebook File: Plant_Disease_Detection.ipynb

🎥 Demo Video: Watch Now

🚀 Developed as part of the Tamizhan Skills Rise Internship Program under the domain of Machine Learning & AI.
