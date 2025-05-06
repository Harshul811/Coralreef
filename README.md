This code is part of ongoing research by Harshul Gupta. Unauthorized use or redistribution without explicit permission is prohibited.

# Coral Bleaching Detection using CNN

This repository contains a Colab-based implementation for detecting coral bleaching using Convolutional Neural Networks (CNNs). The notebook processes image data, prepares it for training, and builds a CNN model using TensorFlow/Keras.

## Directory Structure

```
project_root/
├── code.ipynb               # Main Jupyter notebook with full workflow
├── README.md                # This file
└── coral_data/              # Unzipped dataset (created when you run the notebook)
    ├── Train/
    │   ├── Bleached/
    │   └── Unbleached/
    └── ...
```

> The dataset is automatically downloaded and extracted via the Kaggle CLI.

## How to Run the Code

1. **Open in Google Colab**:
   Upload and open `code.ipynb` in Google Colab.

2. **Install and Authenticate Kaggle**:
   - Run the first cell to install the Kaggle CLI.
   - Upload your `kaggle.json` API key file when prompted. You can download it from your Kaggle [account page](https://www.kaggle.com/account).

3. **Download Dataset**:
   The script downloads the "Bleached Corals Detection" dataset from Kaggle and extracts it.

4. **Organize Data**:
   The code splits the dataset into `train`, `val`, and `test` sets.

5. **Train the Model**:
   The CNN model is trained on the training set and evaluated on the validation/test sets.

6. **Output**:
   The model's training and validation accuracy/loss are plotted. Final evaluation metrics may also be shown.

## Dependencies

The following Python packages are required (Colab has most pre-installed):

- `tensorflow`
- `os`, `shutil`, `random` (standard libraries)
- `kaggle` (installed via `pip` in the notebook)
- `google.colab` (for file upload in Colab)

## Setup Instructions

If you're running this **outside Colab**, you’ll need to:
- Install dependencies manually (`pip install kaggle tensorflow`)
- Move your `kaggle.json` to `~/.kaggle/kaggle.json`
- Ensure the dataset is manually downloaded and unzipped.

## Dataset

- Dataset: [Bleached Corals Detection](https://www.kaggle.com/datasets/sonainjamil/bleached-corals-detection)

