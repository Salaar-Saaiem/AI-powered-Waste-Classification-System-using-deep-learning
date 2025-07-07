![Visitor Count](https://visitor-badge.laobi.icu/badge?page_id=Salaar-Saaiem.Garbage-Classification-using-ML)
<br>
# 🗑 Smart Waste Segregation using EfficientNet + Custom CNN (Garbage Classification)

A deep learning project that classifies waste images into 6 recyclable categories using a hybrid CNN model built by fine-tuning EfficientNetV2B2 with custom Convolutional Neural Network layers. The project includes a web-based interface using Gradio with support for image upload and real-time webcam capture.

---
## Target Classes

- 📦 Cardboard  
- 🧪 Glass  
- ⚙️ Metal  
- 📄 Paper  
- 🧴 Plastic  
- 🚮 Trash 
---
## Live Demo

Try the project directly on Hugging Face Spaces without downloading anything:

[![Hugging Face Space](https://img.shields.io/badge/HuggingFace-Demo-blue?logo=huggingface)](https://huggingface.co/spaces/Salaar-Saaiem/Ai-Based_Garbage_Classification_using_ML)

Watch the DEMO here 

[![Watch Demo](https://img.shields.io/badge/🎬-Watch%20Demo-blue?style=for-the-badge)](https://www.linkedin.com/posts/salaarsaaiem525_machinelearning-deeplearning-computervision-activity-7347607976746147840-Biun?utm_source=share&utm_medium=member_desktop)



---

## Features

-  **Hybrid Architecture** – Combines EfficientNetV2B2 with fine-tuned custom CNN layers for superior accuracy and robustness.
-  **Transfer Learning Enabled** – Uses pre-trained EfficientNet weights for faster convergence and better generalization.
-  **High-Precision Garbage Classification** – Classifies waste into six categories: Cardboard, Glass, Metal, Paper, Plastic, and Trash.
-  **Webcam + Upload Prediction** – Real-time prediction using either webcam or uploaded image directly in browser (via Gradio).
-  **Live Inference via Gradio UI** – Seamless user interface for testing any image instantly, no code required.
-  **Performance Monitoring** – Includes loss/accuracy graphs, learning curves, and training logs.
-  **Confusion Matrix** – Visual breakdown of model predictions vs true labels.
-  **Detailed Classification Report** – Outputs precision, recall, F1-score for each class.
-  **Model Persistence** – Easily save and reload the best performing `.keras` models.
-  **Organized Dataset Pipeline** – Structured training/validation/test data loading with augmentation.
-  **Code Modularity** – Separated files for training, deployment, evaluation, and webcam utility.

---
## ⚙️ Model Architecture 

<p align="center">
  <img src="https://github.com/Salaar-Saaiem/Garbage-Classification-using-ML/blob/main/Assets/Architecture Diagram.png" alt="Accuracy & Loss" width="700"/>
</p>
<p>
The visual above represents the complete training and evaluation pipeline. It uses EfficientNetV2B2 as a feature extractor, followed by custom CNN layers. The model is initially trained with a frozen base, then fine-tuned, and finally evaluated on multiple metrics like accuracy, loss curves, and confusion matrix.
</p>

## 🧩 Model Flow Diagram

<p align="center">
  <img src="https://github.com/Salaar-Saaiem/Garbage-Classification-using-ML/blob/main/Assets/Flow%20Diagram.png?raw=true" alt="Model Flow Diagram" width="700"/>
</p>

---
## 📊 Model Evaluation

### Accuracy & Loss Curves

These graphs show how the model improved during training:

<p align="center">
  <img src="https://github.com/Salaar-Saaiem/Garbage-Classification-using-ML/blob/main/Assets/Performance.png" alt="Accuracy & Loss" width="700"/>
</p

- **Left (Accuracy):** Training accuracy steadily improves and validation accuracy stabilizes above **95%**, indicating effective learning and generalization.
- **Right (Loss):** Both training and validation loss decrease rapidly and flatten out, showing that the model is converging without overfitting.

---

### Confusion Matrix

The confusion matrix below summarizes the model’s performance on the test set:

<p align="center">
  <img src="https://github.com/Salaar-Saaiem/Garbage-Classification-using-ML/blob/main/Assets/Confusion Matrix.png" alt="Confusion Matrix" width="700"/>
</p

- High diagonal values (true positives) indicate strong classification accuracy across all six categories: **cardboard, glass, metal, paper, plastic, trash**.
- Minimal confusion is observed between similar classes (e.g., glass and metal).
- Especially strong results for **paper** and **plastic**, with 53 and 46 correct predictions respectively.

---
### Model Predictions 

Following are the test results showing the model predictions on sample images from the test dataset. All predictions below are correct, reflecting the model's high accuracy and generalization capability across multiple garbage classes:

<p align="center">
  <img src="https://github.com/Salaar-Saaiem/Garbage-Classification-using-ML/blob/main/Assets/Testing.png" alt="Model Prediction" width="700"/>
</p>

<p align="center">
  <img src="https://github.com/Salaar-Saaiem/Garbage-Classification-using-ML/blob/main/Assets/Testing2.png" alt="Model Prediction" width="700"/>
</p>

<p align="center">
  <img src="https://github.com/Salaar-Saaiem/Garbage-Classification-using-ML/blob/main/Assets/Testing3.png" alt="Model Prediction" width="700"/>
</p>


---


## Tech Stack

-  **TensorFlow / Keras** – Core deep learning framework used for building, training, fine-tuning, and saving models.
-  **EfficientNetV2B2** – Transfer learning backbone pre-trained on ImageNet, integrated for better performance and faster convergence.
-  **Custom CNN Layers** – Tailored layers added over EfficientNet for domain-specific fine-tuning and improved accuracy.
-  **tf.keras.preprocessing & ImageDataGenerator** – For real-time image augmentation, scaling, and train-validation-test pipeline.
-  **Matplotlib & Seaborn** – For visualizing performance metrics like learning curves, confusion matrix, and prediction results.
-  **Scikit-learn** – For generating classification reports, precision, recall, and F1-score.
-  **Gradio** – For browser-based UI that supports both image upload and live webcam input for real-time predictions.
-  **Python 3.10** – Programming language used throughout the entire project.
-  **NumPy & Pandas** – For efficient numerical operations and dataset handling.
-  **Jupyter Notebook** – For model experimentation, prototyping, and performance evaluation.



---

## 📄 Ownership & License

This project is the intellectual property of [Saaiem Salaar](https://www.linkedin.com/in/salaarsaaiem525) and is licensed under the [MIT License](LICENSE). This means you are free to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the software for personal or commercial purposes, provided that proper credit is given and the original license and copyright notice are included in all copies or substantial portions of the software. The software is provided "as is", without any warranty of any kind, express or implied, and the author is not liable for any claims, damages, or other liabilities arising from its use.
