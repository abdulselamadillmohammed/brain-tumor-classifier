# 🧠 CNN Practice: FashionMNIST ➔ Brain Tumor MRI Classification (PyTorch)

This project starts by practicing convolutional neural networks (CNNs) on the standard FashionMNIST dataset to verify model setup and training techniques.

After verifying functionality, the same CNN design is extended and adapted to a real-world medical imaging problem: **classifying brain tumor MRI scans** into four categories:

- **Glioma**
- **Meningioma**
- **Pituitary Tumor**
- **No Tumor**

The entire workflow is implemented in PyTorch.

---

## 📚 Project Phases

1. **Phase 1: FashionMNIST Practice**
   - Build and train a basic CNN on the FashionMNIST clothing dataset.
   - Verify model performance and understand data transformations.
2. **Phase 2: Brain Tumor MRI Classification**
   - Adapt the CNN to work with grayscale MRI images.
   - Train the model to classify MRI brain scans into tumor types.
   - Visualize predictions with correct/incorrect color-coding.

---

## 📦 Dataset Information

- **FashionMNIST**: Built-in torchvision dataset, 10 classes of clothing items.
- **Brain Tumor MRI Dataset**: [Kaggle link](https://www.kaggle.com/datasets/esfiam/brain-tumor-mri-dataset)
  - Four classes: glioma, meningioma, pituitary tumor, and no tumor
  - Images organized into `train/` and `test/` directories by tumor type
  - Downloaded and extracted using the Kaggle API

---

## 🛠️ How to Run

1. Install required libraries:
    ```bash
    pip install torch torchvision matplotlib kaggle
    ```

2. Download the Brain Tumor MRI Dataset:
    - Follow Kaggle API setup instructions.
    - Use the script provided inside the notebook to download and unzip the dataset.

3. Open and run the notebook:
    - Train the CNN first on FashionMNIST.
    - Then retrain the adapted CNN on the brain tumor MRI dataset.

4. Visualize model predictions with green (✅ correct) and red (❌ incorrect) labeling.

---

## 🚀 Model Details

- **Architecture**: 3 Convolutional layers + ReLU + MaxPooling + Dropout
- **Loss Function**: CrossEntropyLoss
- **Optimizer**: Adam
- **Input Size**: Grayscale images resized to 128x128 pixels
- **Performance**:
  - FashionMNIST: >90% accuracy
  - Brain Tumor MRI: ~86% validation accuracy in 5 epochs

## 🙋‍♀️ Credits

- Dataset by @esfiam on Kaggle

