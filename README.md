# Pneumonia Detection using Deep Learning

## Overview

This project implements a deep learning model for detecting pneumonia from chest X-ray images using transfer learning with the ResNet50 architecture. The model is trained to classify X-ray images into two categories: normal and pneumonia.

## Dataset

The dataset used for this project is sourced from Kaggle. You can find it [here](https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia). The dataset consists of chest X-ray images for training, validation, and testing.

### Dataset Structure

The dataset is organized into three main folders:
- `train/` - Contains images for training.
- `val/` - Contains images for validation.
- `test/` - Contains images for testing.

## Requirements

To run this project, you will need the following packages:

- TensorFlow (version 2.12.0)
- NumPy (version 1.21.0)
- Matplotlib (version 3.4.3)
- Seaborn (version 0.11.2)
- Scikit-learn (version 1.0.2)
- Pillow (version 8.4.0)

You can install the required packages using pip:

```bash
pip install -r requirements.txt
```

## Usage

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Sarath-peddireddy/PneumoniaDetectionProject.git
   cd PneumoniaDetectionProject
   ```

2. **Download the dataset from Kaggle** and extract it to the correct directory structure.

3. **Run the training script:**
   ```bash
   python src/pneumonia_detection_model.py
   ```

4. The model will train on the dataset and save the best model weights in `best_model.keras`.

5. To make predictions on new X-ray images, use the provided prediction function in the script.

## Evaluation

After training, the model's performance is evaluated using test accuracy, loss, classification report, confusion matrix, and ROC curve.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.