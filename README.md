# CNN-Based Waste Segregation System

This project implements a Convolutional Neural Network (CNN) to classify waste materials into 7 categories for improving recycling efficiency and waste management.

## Project Overview

**Student:** Kotresh T M  
**Assignment:** CNN-Based Waste Segregation for Improving Waste Management  
**Date:** May 2026

## Problem Statement

Improper waste disposal leads to environmental degradation and inefficient recycling. This project uses deep learning to automate waste classification, reducing manual labor and improving sorting accuracy.

## Dataset

The dataset contains approximately 7,625 images across 7 waste categories:
- Cardboard
- Food Waste
- Glass
- Metal
- Other
- Paper
- Plastic

## Implementation

### Model Architecture
- 3 Convolutional layers (32, 64, 128 filters)
- Batch Normalization
- MaxPooling layers
- Dropout layers (0.5, 0.3)
- Dense layers (256, 128 neurons)
- Output layer with 7 classes (softmax)

### Key Features
- Image preprocessing and normalization
- Data augmentation (rotation, shifting, flipping, zoom)
- Class imbalance handling
- Comprehensive evaluation metrics

## Results

The model was trained for 15 epochs with:
- Train-validation split: 80-20
- Batch size: 32
- Optimizer: Adam
- Loss function: Categorical Crossentropy

Evaluation metrics include:
- Accuracy
- Precision, Recall, F1-score (per class)
- Confusion Matrix

## Files

- `CNN_Assg_Waste_Segregation_Starter.ipynb` - Main Jupyter notebook with implementation
- `data/` - Dataset folder (not included in submission)

## How to Run

1. Clone this repository
2. Install required libraries:
   ```
   pip install numpy pandas matplotlib seaborn pillow tensorflow scikit-learn
   ```
3. Place the dataset in the `data/` folder
4. Open and run the Jupyter notebook:
   ```
   jupyter notebook CNN_Assg_Waste_Segregation_Starter.ipynb
   ```

## Requirements

- Python 3.x
- NumPy 1.26.4
- Pandas 2.2.2
- Matplotlib 3.10.0
- Seaborn 0.13.2
- PIL 11.1.0
- TensorFlow 2.18.0
- Keras 3.8.0
- Scikit-learn 1.6.1

## Applications

- Smart Recycling Bins
- Automated Waste Sorting Facilities
- Waste Monitoring and Reporting Systems

## Future Improvements

- Address class imbalance with advanced techniques
- Experiment with transfer learning (VGG, ResNet)
- Collect more data for underrepresented classes
- Deploy as a real-time classification system

## License

This project is created for educational purposes as part of an academic assignment.
