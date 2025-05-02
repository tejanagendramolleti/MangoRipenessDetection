# 🥭 Mango Ripening Stage Classification with PyTorch Lightning

This repository contains code for classifying mango ripening stages using deep learning. The models are trained on a public dataset from Kaggle, leveraging various convolutional neural network architectures including:

- Custom CNN
- VGG16
- InceptionV3
- MobileNetV2
- EfficientNet
- DenseNet121

All models are implemented using **PyTorch Lightning** for cleaner training loops and scalability.

---

## 📊 Dataset

**Kaggle Source:**  
[Mango Ripening Stage Classification](https://www.kaggle.com/datasets/srabon00/mango-ripening-stage-classification)

- Three classes:
  - `Unripe`
  - `Semi-Ripe`
  - `Ripe`
- Format: ImageFolder-compatible directory of images.

---

## 🧠 Models & Architectures

Each model uses a standard transfer learning pipeline with frozen feature extractors and a custom classification head:

| Model         | Pretrained | Input Size | Output | Notes                     |
|---------------|------------|------------|--------|---------------------------|
| Custom CNN    | ❌         | 224×224    | 3      | Simple ConvNet            |
| VGG16         | ✅         | 224×224    | 3      | Modified final FC layer   |
| InceptionV3   | ✅         | 299×299    | 3      | Includes aux classifier   |
| MobileNetV2   | ✅         | 224×224    | 3      | Lightweight architecture  |
| EfficientNetB0| ✅         | 224×224    | 3      | Accurate & efficient      |
| DenseNet121   | ✅         | 224×224    | 3      | Good balance of depth     |

---

## 🛠️ Setup Instructions

1. Clone the repo:
```
git clone https://github.com/your-username/mango-ripening-stage-classification.git
cd mango-ripening-stage-classification
```

## Results
![image](https://github.com/user-attachments/assets/4839ddde-e269-4604-9246-7dc5ed3fda61)
