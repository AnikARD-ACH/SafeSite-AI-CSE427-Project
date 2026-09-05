# SafeSite AI: Automated Construction-Site Safety Monitoring

## CSE427 Machine Learning Project

SafeSite AI is an AI-based construction-site safety monitoring system that combines object detection with rule-based spatial reasoning to identify PPE compliance and safety risks.

The system detects construction workers, personal protective equipment (PPE), and machinery from site images and generates interpretable safety compliance decisions.

---

# Project Overview

Construction-site safety monitoring often depends on manual supervision, which is difficult to scale and maintain consistently.

SafeSite AI addresses this problem by developing an automated computer vision pipeline consisting of:

- Multi-source construction safety dataset preparation
- Annotation verification and standardisation
- Class mapping and dataset balancing
- YOLO-based object detection
- Model performance comparison
- Spatial association between workers and PPE
- Rule-based safety risk scoring

---

# Dataset

The final unified dataset contains six object classes:

| Class | Description |
|---|---|
| Person | Construction workers |
| Helmet | Workers wearing helmets |
| No Helmet | Workers without helmets |
| Vest | Workers wearing safety vests |
| No Vest | Workers without safety vests |
| Machinery | Construction equipment |

The dataset preparation process included:

- Dataset acquisition from multiple public sources
- Label verification
- Class vocabulary standardisation
- YOLO annotation format conversion
- Duplicate image removal
- Dataset validation
- Train/validation/test splitting

---

# Methodology

The complete workflow consists of:

Dataset Collection
↓
Annotation Verification
↓
Class Standardisation
↓
Dataset Validation
↓
YOLO Model Training
↓
Performance Evaluation
↓
Spatial Association
↓
Safety Risk Scoring




---

# Machine Learning Models

Five YOLO architectures were trained and compared under identical conditions:

- YOLOv8n
- YOLOv11n
- YOLOv10n
- YOLOv5n
- YOLOv8s

Evaluation metrics include:

- Precision
- Recall
- mAP@50
- mAP@50-95

The best-performing model was selected based on overall detection performance.

---

# Repository Structure

```
SafeSite-AI-CSE427-Project/

├── Safesite AI/
│   └── CSE427_project2.ipynb

├── Report/
│   └── Project report PDF

├── Results/
│   ├── Model Comparison.png
│   ├── confusion_matrix.png
│   ├── class_distribution.png
│
│   ├── Table/
│   │   ├── Safesite_final_dataset_class_distribution_Table.png
│   │   └── unified_class_distribution_table.png
│
│   └── detection examples/
│       ├── val_batch0_pred.jpg
│       ├── val_batch1_pred.jpg
│       └── val_batch2_pred.jpg

├── README.md
├── LICENSE
└── .gitignore
```

# Results

The Results folder contains:

### Dataset Analysis
- Class distribution visualization
- Unified dataset distribution table
- Train/validation/test split analysis

### Model Evaluation
- YOLO model comparison
- Confusion matrix analysis

### Detection Results
- Example prediction outputs with bounding boxes and confidence scores

---

# Technologies Used

- Python
- Google Colab
- YOLO Object Detection
- Computer Vision
- Machine Learning
- OpenCV
- Ultralytics YOLO Framework

---

# Team Members

## Anik Rahman

Contributions:

- Reviewed research papers related to construction safety monitoring
- Built the unified dataset pipeline
- Performed dataset acquisition
- Verified annotations
- Implemented class mapping
- Balanced and validated the dataset
- Converted annotations into YOLO format
- Performed duplicate removal
- Created train/validation/test splits


## Abyaad Zafer Khan

Contributions:

- Reviewed related research papers
- Conducted exploratory data analysis
- Trained and compared multiple YOLO detection models
- Implemented spatial association logic
- Developed rule-based risk scoring layer
- Created the methodology workflow

---

# Project Report

The complete project documentation is available in the `Report/` directory.

---

# Dataset Access

The dataset is provided separately through Google Drive due to its large size.

Dataset access link:
[here](https://docs.google.com/document/d/1fMxVy-JWAIqYYrtbvHSb4gJ1jVchGW-ikvAd92HJ30U/edit?tab=t.wlfrrndlzj)
