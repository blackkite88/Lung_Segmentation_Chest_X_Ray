# Lung Segmentation on Chest X-Rays

## 📌 Overview
This project focuses on **automated lung segmentation from chest X-ray images** using deep learning. Accurate lung segmentation plays a crucial role in medical image analysis, assisting in disease detection, diagnosis, and monitoring.

The repository provides:
- Data preprocessing and augmentation utilities
- Deep learning model for lung segmentation (U-Net based)
- Training and evaluation scripts
- Inference pipeline to generate segmentation masks on new X-ray images

---

## 📂 Repository Structure
```bash
├── load_data.py # Data loading & preprocessing
├── build_model.py # Model architecture (e.g., U-Net)
├── train_model.py # Training script
├── inference.py # Inference / prediction script
├── utils/ # Helper functions
├── requirements.txt # List of dependencies
└── README.md # Project documentation
```

---

## ⚙️ Installation

Clone the repository:
```bash
git clone https://github.com/Kartikboxi/Lung-Segmentation-Chest-X-Ray.git
cd Lung-Segmentation-Chest-X-Ray
```

Install dependencies:

```bash
pip install -r requirements.txt
```
## 📊 Dataset
This project can be trained on publicly available chest X-ray datasets such as:

Montgomery County X-ray Set

JSRT Dataset

Download the dataset manually and place it in the data/ directory.
Update paths in load_data.py accordingly.

## 🚀 Usage
Training

Copy code
```bash
python train_model.py --data_dir ./data --epochs 50 --batch_size 8
```
Inference
```bash
python inference.py --model checkpoints/best_model.h5 --input sample_xray.png --output mask.png
```
## 📈 Results
Achieved Dice coefficient ≈ 0.95.

Example segmentation:

Input X-ray	Predicted Mask

## 📌 Future Work
Improve model generalization with more diverse datasets

Experiment with attention U-Net / transformer-based models

Deploy as a web app for real-time lung segmentation

## 🤝 Contributing
Pull requests are welcome. For significant changes, please open an issue first to discuss what you would like to improve.

# Lung_Segmentation_Chest_X_Ray
