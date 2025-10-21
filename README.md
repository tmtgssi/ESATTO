# Lightweight-Oriented Classification Using Distillation Learning and Spatial Information from Tabular Data

This repository accompanies the project:

> **"Lightweight-Oriented Classification Using Distillation Learning and Spatial Information from Tabular Data"**

The goal is to improve classification performance on tabular datasets using synthetic spatial representations and knowledge distillation. A lightweight student model is trained to mimic a heavier teacher model while utilizing spatial features generated from raw tabular data.

---

## 📂 Contents

- 🔬 `train_teacher.ipynb` — Train a high-capacity teacher model.
- 🧠 `distillation_train.ipynb` — Train a compact student model via distillation.
- 🧪 `distillation_test.ipynb` — Evaluate classification accuracy and visualize performance.
- 🧬 `syn_vision_gen.ipynb` — Generate synthetic image-like data from tabular inputs.

---

## 📦 Dataset and Pretrained Models

### 📁 Synthetic Datasets
You can download the synthetic datasets used in the experiments here:

👉 **[Download Synthetic Datasets](https://drive.google.com/drive/folders/1gKbiHtOFnkVBPohg-dkmBrMisHuBY0KI?usp=sharing)**  

### 🧠 Pretrained Models
Download pretrained teacher and student models here:

👉 **[Download Pretrained Weights](https://drive.google.com/drive/folders/1gKbiHtOFnkVBPohg-dkmBrMisHuBY0KI?usp=sharing)**  

After downloading, extract the files into the project directory as follows:

project-root/

├── syn_vision_dataset/

│ └── [your datasets here]

├── checkpoints/

│ └── [best_model.pth,best_model_res152_dif_p1.pth]


---

## ⚙️ Environment Setup

We recommend using a virtual environment (`conda` or `venv`) and installing dependencies via `pip`.

### 🐍 Python Version
```text
absl-py==2.1.0
torch==2.5.0
torchvision==0.20.0
tensorflow==2.9.0
scikit-learn-intelex==20230228.214242
timm==1.0.15
lightgbm==4.5.0
pytorch-lightning==2.5.1.post0
pandas==2.2.3
numpy==1.26.0
matplotlib

🚀 How to Run
✅ 1. Verify Results
Open and run distillation_test.ipynb inside each experiment folder to verify performance using pretrained weights.

🏋️ 2. Train Models from Scratch
Step 1: Train Teacher

python
Copy code
# Run this notebook
train_teacher.ipynb
Step 2: Train Student with Distillation

python
Copy code
# Run this notebook
distillation_train.ipynb

🧬 🚀 How to Generate Synthetic Data
To create image-like spatial representations from tabular data:

python
Copy code
# Run this notebook
syn_vision_gen.ipynb

📧 Contact
If you have questions or need assistance, feel free to contact:

Minh Trieu Tran
📨 minhtrieu.tran@gssi.it


