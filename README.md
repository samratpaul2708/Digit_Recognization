# 🖋 Digit Recognition using CNN (MNIST Dataset)

## 📌 Overview
This project implements a **Convolutional Neural Network (CNN)** using **TensorFlow** and **Keras** to classify digits from the MNIST dataset.  
The model is trained on 60,000 digit images and tested on 10,000 digit images, achieving high accuracy.

---

## 📂 Dataset
- **MNIST** dataset contains:
  - 60,000 training images
  - 10,000 testing images  
- Image details:
  - Grayscale  
  - 28×28 pixels  
  - Digits labeled from **0 to 9**

---

## ⚙ Steps in the Project
1. **Load Dataset** – MNIST dataset is loaded directly from Keras.
2. **Preprocessing** –  
   - Normalize pixel values (0–255 → 0–1)  
   - Reshape data for CNN input  
   - One-hot encode labels  
3. **Build the Model** –  
   - 2 convolutional layers with max pooling  
   - Flatten layer  
   - Dense + Dropout layer for regularization  
4. **Compile Model** – Using Adam optimizer & categorical crossentropy loss.
5. **Train Model** – Trained for 8 epochs with 10% validation split.
6. **Evaluate Model** – Test accuracy printed at the end.

---

## 🏗 Model Architecture
| Layer           | Description                                   |
|-----------------|-----------------------------------------------|
| Conv2D          | 32 filters, (3×3), ReLU activation            |
| MaxPooling2D    | Pool size (2×2)                               |
| Conv2D          | 64 filters, (3×3), ReLU activation            |
| MaxPooling2D    | Pool size (2×2)                               |
| Flatten         | Flatten into 1D vector                        |
| Dense           | 128 units, ReLU activation                    |
| Dropout         | 50% dropout rate                              |
| Dense (Output)  | 10 units, Softmax activation                  |

---

## 📊 Results
- **Epochs:** 8  
- **Batch size:** 32  
- **Validation split:** 0.1  

### ✅ Accuracy
- **Test Accuracy:** `99%` *(replace with your actual result)
