
# 🐾 CNN for Cat and Dog Image Classification using ResNet-50

An end-to-end Deep Learning project for classifying images of cats and dogs using Transfer Learning with the **ResNet-50** architecture. The notebook includes comprehensive data augmentation and preprocessing steps to maximize validation accuracy.

---

## 🚀 Features
* **Transfer Learning:** Utilizing pretrained ResNet-50 weights from ImageNet.
* **Data Augmentation:** Implemented rotation, zooming, flipping, and shearing using TensorFlow/Keras to prevent overfitting.
* **Evaluation Metrics:** Includes accuracy/loss curves and confusion matrix visualization.

---

## 🛠️ Requirements & Setup

To run this notebook locally or on Google Colab, you need the following libraries:

```python
pip install tensorflow numpy matplotlib scikit-learn
```

### Dataset Structure
Ensure your dataset is organized as follows before running the code:
```text
dataset/
├── train/
│   ├── cats/
│   └── dogs/
└── validation/
    ├── cats/
    └── dogs/
```

---

## 💻 How to Run

1. **Open in Google Colab:** Upload the `Data_ogmantation.ipynb` notebook to your Google Drive and open it via Colab.
2. **Enable GPU:** Go to `Runtime` > `Change runtime type` > Select `T4 GPU` (or any available GPU) for faster training.
3. **Download Dataset:** Mount your Google Drive or download your dataset directly into the workspace.
4. **Execute Cells:** Run the cells sequentially to preprocess data, build the model, and begin training.

---

## 📊 Model Architecture & Training

* **Base Model:** ResNet-50 (Frozen core with Custom GlobalAveragePooling2D).
* **Dense Layers:** Fully connected layers with ReLU activation and Dropout (0.5) to avoid overfitting.
* **Output Layer:** Sigmoid activation for binary classification (Cat vs. Dog).
* **Optimizer:** Adam Optimizer.
* **Loss Function:** Binary Crossentropy.

---

## 📈 Results

* **Training Accuracy:** ~98% (Achieved via Transfer Learning)
* **Validation Accuracy:** Highly optimized using advanced data augmentation technique variations.

---

## 🤝 Contributing
Contributions, issues, and feature requests are welcome! Feel free to check the issues page if you want to contribute to this project.
