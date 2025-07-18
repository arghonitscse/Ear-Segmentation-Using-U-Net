# Ear-Segmentation-Using-U-Net

This project was developed as part of my Summer research internship, at NIT SILCHAR under Proffesor Debbrota Paul Choudhury, focusing on semantic segmentation using deep learning. It implements a U-Net model with a ResNet-34 encoder to perform pixel-wise ear segmentation on the AWEForSegmentation dataset, achieving strong IoU and Dice scores.


## 📁 Dataset: AWEForSegmentation

- Annotated ear segmentation dataset
- Used folders:
  - `train/` — original facial images
  - `trainannot/` — corresponding binary masks (1 for ear, 0 for background)
- Images were resized to 256×256 for training

---

## 🧠 Model Overview

| Feature        | Value                        |
|----------------|------------------------------|
| Architecture   | U-Net with ResNet-34 encoder |
| Input Channels | 3 (RGB)                      |
| Output Classes | 1 (binary segmentation)      |
| Activation     | Sigmoid                      |
| Loss Function  | Dice + Binary Cross Entropy  |

Trained using PyTorch and segmentation_models_pytorch.

---

## 🧪 Training Configuration

- **Input Size:** 256 × 256  
- **Batch Size:** 4  
- **Epochs:** 7  
- **Optimizer:** Adam (`lr=1e-4`)  
- **Evaluation Metrics:** IoU Score, Dice Score

---

## 📊 Results

| Metric   | Score   |
|----------|---------|
| **IoU**  | 0.8317  |
| **Dice** | 0.9081  |

---

## 🚀 Tools & Libraries

- Python (Colab)
- PyTorch
- OpenCV
- `segmentation_models_pytorch`
- Matplotlib

---

## 🔭 Future Directions

- Train with **augmented or rectified masks**
- Convert model to ONNX or TFLite for deployment
- Build a mobile app (Flutter) for real-time ear detection
- Improve generalization with data augmentation

---

## 👨‍💻 Author

Developed during my **2025 research internship**  
Focus: **deep learning for biometric segmentation**
