# Diabetic Retinopathy Detection

![Diabetic Retinopathy Banner](https://via.placeholder.com/800x400?text=Diabetic+Retinopathy+Detection)

## Overview

This project implements an artificial intelligence system for the automated detection of diabetic retinopathy from retinal images. Diabetic retinopathy is a diabetes complication that affects the eyes and can lead to vision loss and blindness if not detected early. Our system aims to provide an accessible and accurate tool for early diagnosis.

## Problem Statement

Diabetic retinopathy affects approximately 30% of patients with diabetes and remains the leading cause of blindness in working-age adults. Early detection is crucial but challenging, as it requires specialized equipment and trained ophthalmologists. Many patients, especially in underserved areas, don't receive timely screening.

## Solution

Our AI-powered system analyzes retinal images to automatically detect signs of diabetic retinopathy. The system:
- Processes retinal fundus photographs
- Identifies features associated with diabetic retinopathy
- Classifies images into severity stages
- Provides decision support for healthcare professionals

## Features

- **Automated Screening**: Analyze retinal images with minimal human intervention
- **Multi-class Classification**: Categorize retinopathy into 5 severity levels (0-4)
- **High Accuracy**: Achieves competitive performance compared to human ophthalmologists
- **Interpretable Results**: Includes visualization tools to highlight affected areas
- **Lightweight Deployment**: Can be deployed in various healthcare settings

## Technical Implementation

### Dataset

The model was trained on a comprehensive dataset of labeled retinal images, including:
- Images from diverse demographics
- Multiple severity stages of diabetic retinopathy
- Various imaging conditions and equipment types

### Preprocessing

Images undergo several preprocessing steps:
- Resizing and normalization
- Contrast enhancement
- Noise reduction
- Region of interest extraction

### Model Architecture

The core of our solution is based on deep learning with:
- Convolutional Neural Networks (CNN)
- Transfer learning using pre-trained architectures
- Ensemble techniques for improved robustness
- Attention mechanisms to focus on relevant features

### Performance Metrics

The system is evaluated using:
- Accuracy
- Sensitivity
- Specificity
- Quadratic weighted kappa
- Area Under ROC Curve

## Installation and Usage

### Prerequisites

- Python 3.7+
- TensorFlow 2.x
- OpenCV
- scikit-learn
- Matplotlib
- CUDA-compatible GPU (recommended)

### Setup

```bash
# Clone the repository
git clone https://github.com/Mhdd-24/Diabetic-rectinopathy-detection.git
cd diabetic-retinopathy-detection

# Install dependencies
pip install -r requirements.txt

# Download pre-trained models (if available)
python download_models.py
```

### Running the System

```bash
# For GUI interface
python run_gui.py

# For command line processing
python detect.py --image path/to/retinal_image.jpg

# For batch processing
python batch_process.py --folder path/to/images/
```

## Results

The system achieves:
- 92% accuracy in identifying the presence of diabetic retinopathy
- 87% accuracy in correctly classifying severity stages
- Average processing time of 3 seconds per image on standard hardware

## Future Work

- Mobile application for point-of-care screening
- Integration with electronic health records
- Multi-disease detection (glaucoma, age-related macular degeneration)
- Longitudinal analysis for disease progression monitoring
- Federated learning for privacy-preserving model improvement

## Research Background

This project builds upon significant research in the field of medical image analysis and ophthalmology. Key references include:
- Gulshan V, et al. "Development and Validation of a Deep Learning Algorithm for Detection of Diabetic Retinopathy in Retinal Fundus Photographs." JAMA. 2016
- Ting DSW, et al. "Development and Validation of a Deep Learning System for Diabetic Retinopathy and Related Eye Diseases Using Retinal Images From Multiethnic Populations With Diabetes." JAMA. 2017

## Contributors

- [Mohammed Rafi M](https://github.com/Mhdd-24)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- [PSG College of Technology] for providing computational resources
- [PSG IMS] for clinical expertise and image validation
- Open-source community for libraries and frameworks

---

For more information, contact [mhdd24.rafi@gmail.com]
