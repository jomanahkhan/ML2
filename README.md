# Machine Learning Coursework

This repository contains code and documentation for my Machine Learning coursework. The project involves implementing and reproducing results from various active learning experiments on the CIFAR-10 dataset, using a pretrained SimCLR model for feature extraction.

## Overview

1. **Active Learning Experiments**  
   - Implements several strategies (e.g., TypiClust, Random).  
   - Compares accuracy, class distribution, and other metrics across multiple trials.

2. **Feature Extraction**  
   - Uses a pretrained SimCLR model (`simclr_cifar-10.pth.tar`) to extract meaningful representations from CIFAR-10 images.  
   - Embeddings are then used for clustering, labeling, and classification tasks.

3. **Statistical Analysis**  
   - Provides summary statistics (mean, standard deviation) across multiple trials.  
   - Visualizations include line plots of accuracy vs. number of labels, t-SNE projections, and label distribution histograms.

## Requirements

- [Python 3.x](https://www.python.org/downloads/)
- [PyTorch](https://pytorch.org/) (for loading and using the pretrained model)
- [NumPy](https://numpy.org/)
- [Matplotlib](https://matplotlib.org/)
- [scikit-learn](https://scikit-learn.org/stable/) (for clustering, t-SNE, etc.)

> *Note:* Google Colab typically has these libraries preinstalled. If any are missing, install via:
>
> ```bash
> !pip install <package_name>
> ```

## Usage

1. **Open the Code in Google Colab**  
   - Upload the notebook (`.ipynb` file) to your Google Drive or GitHub repository.  
   - Launch Google Colab and open the notebook.

2. **Pretrained SimCLR Model**  
   - Make sure you have the pretrained SimCLR weights file named `simclr_cifar-10.pth.tar`.  
   - Place it in the path:  
     ```
     /content/drive/My Drive/cw2_ML/simclr_cifar-10.pth.tar
     ```
   - Verify the file path in your notebook or scripts, especially if you're mounting Google Drive in Colab.

3. **Running the Code**  
   - Mount your Google Drive in Colab:
     ```python
     from google.colab import drive
     drive.mount('/content/drive')
     ```
   - Confirm that `simclr_cifar_
