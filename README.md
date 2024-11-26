# Lung-Nodule-Detection-using-RCNN
Welcome to my Lung Nodule Detection project! I worked on a team to create an RCNN (Region-Based Convolutional Neural Netowork) that identifies lung nodule in patient lung CT scan using transfer learning.
---

## 📂 Project Structure

### 1. **Data Preparation**
   - **Objective:** Load, preprocess, and split the dataset into training, validation, and test sets.
   - **Key Functions:**
     - `load_data()`: Imports lung nodule dataset.
     - `preprocess_images()`: Applies normalization and resizing.

### 2. **Model Architecture**
   - **Objective:** Define and configure the CNN model using ResNet-50.
   - **Key Components:**
     - Utilizes a **ResNet-50** backbone for feature extraction.
     - Fully connected layers for binary classification (nodule present or absent).

### 3. **Transfer Learning Implementation**
   - **Objective:** Enhance model performance using pre-trained weights from ImageNet.
   - **Steps:**
     - Load pre-trained **ResNet-50** weights.
     - Fine-tune specific layers while retaining general image features.

### 4. **Training Process**
   - **Objective:** Train the model with prepared data and evaluate performance.
   - **Key Functions:**
     - `train_model()`: Executes the training loop with loss calculation.
     - Implements data augmentation for better generalization.

### 5. **Evaluation and Metrics**
   - **Objective:** Assess the model's performance.
   - **Metrics Used:**
     - Accuracy, Precision, Recall, F1-score.
     - ROC-AUC for comprehensive evaluation.

### 6. **Visualization**
   - **Objective:** Provide insights into training results.
   - **Tools:**
     - **Loss and Accuracy Plots**: Monitor training/validation performance.
     - **Confusion Matrix**: Visualize classification results.

### 7. **Deployment/Inference**
   - **Objective:** Apply the trained model to new CT scans for nodule detection.
   - **Functionality:**
     - `predict_nodule()`: Generates predictions on unseen data.

---

## 🔑 Key Features
- **Deep Learning with ResNet-50:** Utilizes a robust pre-trained network for feature extraction.
- **Transfer Learning:** Speeds up training and improves accuracy with fewer labeled samples.
- **Customizable:** Adaptable to different datasets and nodule detection criteria.
