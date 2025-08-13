# 🐶🐱 PetVision — Cats vs Dogs Classifier (TensorFlow Lite)

PetVision is an image classification project built with **TensorFlow**, **MobileNetV2**, and **TensorFlow Lite** to distinguish between cats and dogs.  
The project demonstrates **model training**, **evaluation**, and **quantization** techniques (dynamic range and full integer quantization) for efficient deployment on edge devices.

---

## 📌 Features
- **Dataset**: [`cats_vs_dogs`](https://www.tensorflow.org/datasets/catalog/cats_vs_dogs) from TensorFlow Datasets
- **Model Architecture**: MobileNetV2 + Dense layer
- **Quantization Types**:
  - Dynamic Range Quantization
  - Full Integer Quantization (INT8)
- **Evaluation**:
  - Runs inference on 100 test images
  - Displays classification accuracy
  - Plots prediction results with confidence scores

---

## 📂 Project Structure
```
PetVision/
│
├── pet_vision_model/
│   ├── pet_vision_model.tflite
│   ├── dynamic_optimized_model.tflite
│   ├── integer_optimized_model.tflite
│
├── PetVision.ipynb
└── README.md

```

---

## 🚀 How It Works
1. Load Dataset
2. Build Model
3. Train & Save
4. Quantization

---

📊 Results
Evaluated on 100 test images

Plots show predicted vs actual labels

Quantized models are smaller and faster, with minimal accuracy loss

---

🖼 Sample Output
Predictions Plot

---

📦 Models Exported
Model Type	File Name	Size Reduction
```
FP32 Original	pet_vision_model.tflite	—
Dynamic Range Quantized	dynamic_optimized_model.tflite	✅ Reduced
INT8 Quantized	integer_optimized_model.tflite	✅✅ More Reduced
```
