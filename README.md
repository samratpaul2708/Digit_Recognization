# MNIST Handwritten Digit Classifier 🖊️🔢  

This project is a simple **Neural Network** built using **TensorFlow/Keras** to recognize handwritten digits from the **MNIST dataset** with high accuracy (~97%).  

## 📌 Overview  
The model:  
- Takes **28×28 pixel grayscale images** of digits (0–9) as input.  
- Flattens them into a **784-element vector**.  
- Passes through a **fully connected hidden layer** with ReLU activation.  
- Outputs probabilities for **10 digit classes** using softmax.  

**Test Accuracy Achieved:** ~97.5% ✅  

---

## 🗂 Dataset  
We use the **MNIST dataset** included in `tensorflow.keras.datasets`.  
- **60,000** images for training  
- **10,000** images for testing  

---

## ⚙️ Requirements  
Install the dependencies before running the script:  

```bash
pip install tensorflow
