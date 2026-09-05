# SafeSite AI: Automated Construction-Site Safety Monitoring

## CSE427 Machine Learning Project

SafeSite AI is an AI-based construction safety monitoring system using object detection and rule-based spatial reasoning.

The system detects workers, PPE equipment, and machinery from construction-site images and generates interpretable safety compliance decisions.

## Project Overview

The project workflow includes:

- Dataset acquisition from multiple public sources
- Annotation verification and semantic checking
- Class standardisation
- YOLO format conversion
- Dataset validation and duplicate removal
- Train/validation/test splitting
- YOLO-based object detection model training
- Spatial association and risk scoring

## Dataset Classes

The final dataset contains six classes:

1. Person
2. Helmet
3. No Helmet
4. Vest
5. No Vest
6. Machinery

## Team Members

### Anik Rahman
- Dataset acquisition
- Annotation verification
- Class mapping
- Dataset balancing
- Format conversion
- Deduplication
- Validation and splitting

### Abyaad Zafer Khan
- Literature review
- Exploratory data analysis
- YOLO model training and comparison
- Spatial association
- Risk scoring layer
- Methodology design

## Files

- `notebooks/` → Google Colab implementation
- `report/` → Project report
- `dataset/` → Dataset documentation
- `results/` → Model results and figures

## Technologies

- Python
- Google Colab
- YOLO Object Detection
- Computer Vision
- Machine Learning
