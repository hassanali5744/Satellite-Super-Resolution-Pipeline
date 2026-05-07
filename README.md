# Satellite-SuperResolution

AI-Based Satellite Image Super-Resolution using Deep Learning & Remote Sensing

Enhancing low-resolution satellite imagery into high-resolution outputs using SwinIR and deep learning techniques trained on the WorldStrat Dataset.

---

## Overview

This project focuses on satellite image super-resolution using AI models trained on remote sensing imagery.

The repository contains:

- Training Code
- Dataset Processing Code
- Inference Scripts
- Trained `.pth` Model
- Kaggle Training Notebook
- WorldStrat Dataset Support

The model was trained on Kaggle GPU using PyTorch.

---

## Super-Resolution Pipeline

```text
Low Resolution Image
        ↓
   SwinIR Model
        ↓
 Image Enhancement
        ↓
High Resolution Output
```

---

## Repository Structure

```bash
Satellite-SuperResolution/
│
├── dataset/
├── training/
├── inference/
├── models/
├── notebooks/
├── outputs/
└── README.md
```

---

## Features

- Satellite Image Super-Resolution
- SwinIR-Based Enhancement
- WorldStrat Dataset Support
- Pretrained `.pth` Model Included
- High-Resolution Image Generation
- Kaggle GPU Training

---

## Dataset

This project uses the WorldStrat Satellite Dataset for training and testing.

The dataset contains:
- Low Resolution Satellite Images
- High Resolution Reference Images
- Remote Sensing Terrain Data

---

## Trained Model

The repository includes a pretrained model file:

```bash
high_res_stn_model.pth
```

You can directly load the model and generate high-resolution satellite images.

---

## Installation

Clone the repository:

```bash
git clone https://github.com/your-username/Satellite-SuperResolution.git
cd Satellite-SuperResolution
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## Load Trained Model

```python
import torch

model.load_state_dict(torch.load("high_res_stn_model.pth"))
model.eval()
```

---

## Run Inference

```bash
python inference.py
```

Generate super-resolved images:

```python
sr_image = model(lr_image)
```

---

## Usage

1. Download the `.pth` model file  
2. Run the WorldStrat dataset code  
3. Load the trained model  
4. Run inference/testing classes  
5. Generate high-resolution satellite images  

---

## Technologies Used

- Python
- PyTorch
- OpenCV
- NumPy
- SwinIR
- Remote Sensing
- Kaggle GPU

---

## Research Inspiration

Inspired by the research paper:

*Towards High-Resolution Alignment and Super-Resolution of Multi-Sensor Satellite Imagery* :contentReference[oaicite:0]{index=0}

---

## Author

Hassan Ali  
Computer Science Student  
AI • Deep Learning • Remote Sensing Enthusiast

---

## Future Improvements

- Multi-Spectral Training
- Better Refinement Networks
- Faster Inference
- Real-Time Satellite Super-Resolution

---

## License

This project is for educational and research purposes.
