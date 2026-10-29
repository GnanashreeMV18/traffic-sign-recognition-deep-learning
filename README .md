# Traffic Sign Recognition Using Deep Learning

A computer vision project that explores and classifies German traffic signs using convolutional neural networks (CNNs). The notebook compares a CNN trained with image augmentation, LeNet, and a modified AlexNet architecture.

## Project overview

Traffic sign recognition is a useful computer vision task for driver-assistance and autonomous driving research. This project covers exploratory data analysis, image preprocessing, model training, and evaluation on the **German Traffic Sign Recognition Benchmark (GTSRB)**, which has **43 traffic sign classes**.

## Models and reported results

The accompanying project report lists the following accuracy figures:

| Model | Reported accuracy |
| --- | ---: |
| CNN with data augmentation | **96.90%** |
| Modified AlexNet | 95.27% |
| LeNet | 94.11% |

These figures are reproduced from the supplied project report; see the notebook for training and evaluation details. They have not been independently rerun or verified here.

## What the notebook covers

- Exploration of traffic sign class distribution, image brightness, contrast, size, and colour
- Image preprocessing: resizing, normalization, grayscale conversion, and contrast enhancement
- Image quality analysis, including blur detection using Laplacian variance and Canny edge detection
- CNN training with image augmentation and callbacks
- Model comparison and visualization of learning curves
- Evaluation and predictions on traffic sign images

## Tools and libraries

Python, Jupyter Notebook, TensorFlow/Keras, NumPy, Pandas, Matplotlib, Seaborn, scikit-learn, OpenCV, and KaggleHub.

## Dataset

[GTSRB German Traffic Sign Recognition Benchmark on Kaggle](https://www.kaggle.com/datasets/meowmeowmeowmeowmeow/gtsrb-german-traffic-sign)

The images are not included in this repository. The notebook uses KaggleHub to download the dataset.

## How to explore

1. Open [`G16_Code.ipynb`](G16_Code.ipynb) in GitHub, Jupyter, or Google Colab.
2. Install the required packages:

   ```bash
   pip install numpy pandas matplotlib seaborn tensorflow scikit-learn opencv-python kagglehub
   ```
3. Download the dataset using the KaggleHub step in the notebook.
4. **Before running all cells:** replace the notebook's hard-coded Colab/Kaggle cache paths with your local downloaded dataset path, and adjust the `/content/Models/` save locations as needed. Training three models can take substantial time and compute.

## Files

- `G16_Code.ipynb` — analysis, preprocessing, model training, and evaluation notebook
- `README.pdf` — original project documentation

## Notes

This repository presents an educational machine learning experiment; it is not a production-ready real-time traffic sign detection system.
