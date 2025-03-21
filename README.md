# 📌 Vehicle Classification using Deep Learning

## 📄 Project Overview
This project focuses on classifying vehicle images using deep learning techniques. We utilize three different approaches:
1. **Transfer Learning** – Using pre-trained models such as MobileNetV2 and ResNet50.
2. **Image Retrieval using Embeddings** – Extracting image features and performing KNN-based search.
3. **End-to-End CNN** – Training a custom convolutional neural network (CNN) for classification.

The dataset used is the **Stanford Cars Dataset**, which consists of 16,185 images across 196 car categories. The challenge includes handling class imbalance, variations in image quality, and learning meaningful feature representations.

---

## 📂 Project Structure
```
vehicle-classification-dl/
├── notebooks/             # Jupyter notebooks for different experiments
│   ├── final_project_basics_2025_notebook1.ipynb  # Transfer Learning experiments
│   ├── final_project_basics_2025_notebook2.ipynb  # Image Retrieval experiments
│   ├── final_project_basics_2025_notebook3.ipynb  # End-to-End CNN experiments
│
├── report.pdf             # Final project report
├── README.md              # Project description
├── requirements.txt       # Required Python packages
└── .gitignore             # Prevents unwanted files from being committed
```

---

## 🔍 Dataset & Preprocessing
- The dataset contains **196 classes of cars** with labeled bounding boxes.
- Images were resized and normalized before feeding into models.
- **Data augmentation** (flipping, rotation, color jittering) was applied for improved generalization.

---

## 🧠 Models Used
### 🔹 **Transfer Learning**
- **MobileNetV2** and **ResNet50** were fine-tuned.
- Experimented with freezing/unfreezing layers, different optimizers, and learning rate schedules.

### 🔹 **Image Retrieval using Embeddings**
- Extracted feature embeddings from MobileNetV2, ResNet50, and EfficientNet-B7.
- Used **KNN search** (k=5) to find similar images.
- Applied **PCA** for dimensionality reduction and improved clustering.

### 🔹 **End-to-End CNN**
- Built a custom CNN with **batch normalization, dropout, and adaptive pooling**.
- Applied **learning rate scheduling** and **weight decay** for optimization.

---

## 📊 Model Evaluation
- **Accuracy Metrics**: Top-1 Accuracy, Top-5 Accuracy.
- **Performance Metrics**: Precision, Recall, F1-score.
- **Loss Functions**: Categorical Cross-Entropy.
- **Visualization**: Confusion matrices and loss/accuracy curves.

---

## 🚀 Running the Project
### 1️⃣ Install dependencies
```bash
pip install -r requirements.txt
```

### 2️⃣ Run Experiments
- Open the respective notebook from `notebooks/` and execute it.

### 3️⃣ Evaluate Results
- Check the **report.pdf** and visualizations inside notebooks for model performance.

---

## 🏆 Key Findings
- **Fine-tuned MobileNetV2** performed best in Transfer Learning.
- **EfficientNet-B7 embeddings** yielded the most accurate Image Retrieval results.
- **CNN with Data Augmentation** achieved the best accuracy in the End-to-End approach.

---

