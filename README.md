# Final Year Project

This repository contains the code and resources for my final year project focused on enhancing image classification in fault detection within the steel industry using deep learning and clustering algorithms.

## Repository Structure

- `final_year_project.ipynb`: Main notebook implementing the project using K-Means clustering.
- `project_hierarchical.ipynb`: Notebook implementing the project using Hierarchical clustering.
- `project_dbscan.ipynb`: Notebook implementing the project using DBSCAN clustering.

## Project Overview

The goal of this project is to improve the accuracy and efficiency of fault detection in steel surfaces through high-resolution image processing and advanced clustering methods. The project leverages deep learning for feature extraction and various clustering algorithms for fault detection.

### Key Components

1. **Data Preprocessing**:
   - High-resolution image processing to capture intricate details of steel surfaces.
   - Data augmentation to improve model resilience.

2. **Feature Extraction**:
   - Using pre-trained ResNet-50 model to extract deep features from images.

3. **Clustering Algorithms**:
   - **K-Means Clustering**: Implemented in `final_year_project.ipynb`.
   - **Hierarchical Clustering**: Implemented in `project_hierarchical.ipynb`.
   - **DBSCAN**: Implemented in `project_dbscan.ipynb`.

4. **Model Training and Refinement**:
   - Initial training phase using a standard CNN model.
   - Iterative model improvement through hyperparameter tuning based on clustering results.

5. **Visualization**:
   - Dimensionality reduction using PCA and t-SNE for visualization of clustered features.

## Getting Started

### Prerequisites

- Python 3.x
- PyTorch
- torchvision
- scikit-learn
- PIL (Pillow)
- numpy
- matplotlib

### Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/ochudi/final_year_project.git
    cd final_year_project
    ```

2. Install the required packages:
    ```bash
    pip install torch torchvision scikit-learn pillow numpy matplotlib
    ```

### Usage

1. Open the desired notebook (`final_year_project.ipynb`, `project_hierarchical.ipynb`, or `project_dbscan.ipynb`) in Jupyter Notebook or Jupyter Lab.
2. Run the cells to execute the code. Ensure you have your dataset in the specified path.

### Dataset

The project uses a dataset of steel surface images for fault detection. The dataset should be organized in a folder structure where each sub-folder represents a category of faults. Example:

```
/path/to/dataset/
    ├── defect_type_1/
    │   ├── image1.jpg
    │   ├── image2.jpg
    ├── defect_type_2/
    │   ├── image3.jpg
    │   ├── image4.jpg
    ...
```

## Results

The results include clustered images visualized using t-SNE, with each cluster representing a different type of fault detected in the steel surfaces.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## Acknowledgments

- Thanks to the authors of the libraries used in this project: PyTorch, torchvision, scikit-learn, PIL, numpy, and matplotlib.
- Special thanks to my supervisors and peers for their guidance and support.
