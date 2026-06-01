# 🧠 Advanced Machine Learning Methods for Alzheimer's Disease Classification

A deep learning-based system for automated classification of Alzheimer's Disease (AD) stages using brain MRI scans. This project leverages state-of-the-art convolutional neural networks and transfer learning techniques to assist in the early detection and staging of Alzheimer's Disease.

🏆 Third Place Winner – Graduation Projects Competition, College of Applied Computer Sciences, King Saud University.

---

## 📖 Overview

Alzheimer's Disease (AD) is one of the leading causes of dementia worldwide and significantly affects memory, cognition, and daily functioning. Early diagnosis plays a crucial role in improving patient outcomes and treatment planning.

This project aims to develop an intelligent MRI-based diagnostic support system capable of classifying brain scans into four Alzheimer's Disease stages using deep learning techniques.

The proposed system analyzes structural MRI images and predicts one of the following categories:

- Non-Demented
- Very Mild Demented
- Mild Demented
- Moderate Demented

The project evaluates multiple deep learning architectures and identifies the most effective model for this task.

---

## 🎯 Objectives

- Develop an AI-powered Alzheimer's Disease classification system.
- Utilize MRI scans for non-invasive diagnosis.
- Compare different deep learning architectures.
- Improve classification accuracy through transfer learning.
- Deploy the model through a user-friendly web interface.

---

## 🏗️ Project Architecture

The development process followed three stages:

### Phase 1: SimpleMLP
A baseline Multi-Layer Perceptron model used for initial experimentation.

### Phase 2: ResNet-18
A transfer learning approach using a pre-trained ResNet-18 architecture.

### Phase 3: EfficientNet-B0
The final selected model, achieving the highest performance and computational efficiency.

---

## 🧪 Datasets

### Dataset 1 – Kaggle Alzheimer's MRI Dataset

| Class | Images |
|---------|---------:|
| Non-Demented | 9,600 |
| Very Mild Demented | 8,960 |
| Mild Demented | 8,960 |
| Moderate Demented | 6,464 |
| **Total** | **33,984** |

After balancing:

- Total Images: 38,400

### Dataset 2 – Mendeley MRI Dataset

| Class | Images |
|---------|---------:|
| Non-Demented | 3,200 |
| Very Mild Demented | 2,240 |
| Mild Demented | 896 |
| Moderate Demented | 64 |
| **Total** | **6,400** |

---

## ⚙️ Technologies Used

### Programming Languages

- Python

### Deep Learning Frameworks

- PyTorch
- Torchvision

### Data Processing

- NumPy
- Pandas
- OpenCV

### Visualization

- Matplotlib

### Deployment

- Gradio
- Hugging Face Spaces

### Development Environment

- Jupyter Notebook
- Git
- GitHub

---

## 🧠 Model Configuration

### EfficientNet-B0

```python
Optimizer: AdamW
Learning Rate: 3e-4
Weight Decay: 1e-3
Loss Function: CrossEntropyLoss
Input Size: 224 × 224
Epochs: 5
Batch Size: 64
```

### Data Preprocessing

- Resize MRI images to 224×224
- Convert grayscale MRI images to RGB
- Normalize using ImageNet statistics
- Dataset shuffling
- Reproducible train-test splitting using seed = 42

---

## 📊 Results

### MRI Dataset 1

| Model | Accuracy |
|---------|---------:|
| SimpleMLP | 83.00% |
| ResNet-18 | 94.00% |
| EfficientNet-B0 | **99.75%** |

### MRI Dataset 2

| Model | Accuracy |
|---------|---------:|
| EfficientNet-B0 | **97.77%** |

---

## 🏆 Comparison with Previous Work

| Model | Accuracy |
|---------|---------:|
| ALZENET | 97.31% |
| SVM | 89.84% |
| Inception-ResNet-V2 | 79.12% |
| **Our EfficientNet-B0** | **99.75%** |

The proposed EfficientNet-B0 model achieved the highest classification accuracy among the compared approaches.

---

## 🌐 Deployment

The final model was deployed using:

### Gradio

A lightweight web interface allowing users to upload MRI images and receive predictions instantly.

### Hugging Face Spaces

The application is hosted online for easy access and demonstration.

🔗 Demo Link:

```
https://huggingface.co/spaces/Yousef20/alzheimer-mri-detection
```

---

## 🚀 Installation

Clone the repository:

```bash
git clone https://github.com/yourusername/alzheimer-mri-classification.git
cd alzheimer-mri-classification
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Run the application:

```bash
python app.py
```

---

## 📂 Project Structure

```text
Alzheimer-MRI-Classification/
│
├── app.py
├── train.py
├── predict.py
├── requirements.txt
├── README.md
│
├── models/
│   └── efficientnet_b0.pth
│
├── notebooks/
│   └── experiments.ipynb
│
├── images/
│   ├── confusion_matrix.png
│   ├── accuracy_curve.png
│   └── demo.png
│
├── docs/
│   └── Final_Report.pdf
│
└── dataset/
```

---

## 🔮 Future Work

Potential improvements include:

- Multi-modal learning using MRI + PET scans.
- Longitudinal patient tracking.
- Explainable AI techniques (Grad-CAM, SHAP).
- Larger multi-center datasets.
- Clinical integration.
- Lightweight model optimization for edge deployment.

---

## 👨‍💻 Team Members

- Talal Alshehri
- Yousef Alabri
- Omar Sahhari
- Osama Raed

### Supervisor

Prof. Mohamad Mahmoud Al Rahhal

College of Applied Computer Sciences  
King Saud University

---

## 📜 License

This project is developed for academic and research purposes.

Feel free to use, modify, and extend the work with proper attribution.

---

## 🙏 Acknowledgements

We express our sincere gratitude to:

- Prof. Mohamad Al Rahhal
- College of Applied Computer Sciences
- King Saud University
- Our families, friends, and colleagues for their continuous support throughout this journey.

---

⭐ If you found this project useful, please consider giving the repository a star.
