# Role of Data Normalization for Image Classification 

This project applies data normalization and kernel methods to classify medical images into benign and malignant categories. Using techniques like Kernel PCA and Support Vector Machine (SVM) with RBF kernels, the project achieves high recall for malignant cases, making it potentially useful for early detection in medical diagnostics.

## Table of Contents
1. [Project Overview](#project-overview)
2. [Package Requirements](#package-requirements)
3. [Setup Instructions](#setup-instructions)
4. [Run Instructions](#run-instructions)
5. [Usage and Results](#usage-and-results)

---

### Project Overview
This project focuses on building a reliable image classification model using various normalization techniques and kernel methods. The primary aim is to distinguish between benign and malignant images with high accuracy and recall, essential in medical diagnostics.

### Package Requirements

To replicate the results, you’ll need the following Python packages:

- **Python 3.7+**
- **numpy** - For numerical operations
- **matplotlib** - For data visualization
- **seaborn** - For advanced data visualization
- **PIL (Pillow)** - For image processing
- **scikit-learn** - For machine learning algorithms and metrics
- **tensorflow** - For data handling (if applicable for dataset loading)

You can install these packages using the following command:

```bash
pip install numpy matplotlib seaborn pillow scikit-learn tensorflow
```

### Setup Instructions

1. **Clone the Repository or Download the Code**:
   Clone this repository or download the code as a ZIP file and extract it to your desired location.

   ```bash
   git clone https://github.com/sachinsingh2156/Role_of_data_normalization_for_image_classification.git
   cd Role_of_data_normalization_for_image_classification
   ```

2. **Prepare the Dataset**:
   - Download the dataset of benign and malignant images and organize them in two directories: `benign` and `malignant`.
   - Ensure the directory structure is as follows:
     ```
     dataset/
     ├── benign/
     │   ├── image1.jpg
     │   ├── image2.jpg
     │   └── ...
     └── malignant/
         ├── image1.jpg
         ├── image2.jpg
         └── ...
     ```

3. **Install Required Libraries**:
   Ensure that all required libraries are installed. Use the command below if not done already:

   ```bash
   pip install -r requirements.txt
   ```

   Alternatively, manually install each package as mentioned in the "Package Requirements" section.

### Run Instructions

1. **Open the Jupyter Notebook**:
   - Start Jupyter Notebook by running:
     ```bash
     jupyter notebook
     ```
   - Open the notebook file (`Data_normalization.ipynb`).

2. **Run the Notebook Cells**:
   - The notebook is structured with clear, sequential cells. Run each cell from top to bottom for data loading, preprocessing, model training, evaluation, and visualization.
   - Key steps include:
     - Loading and preprocessing the dataset
     - Applying Min-Max and Z-score normalization
     - Applying Kernel PCA for dimensionality reduction
     - Training and evaluating the SVM model and Random Forest model
     - Displaying evaluation metrics and visualizations, including the confusion matrix and classification report

3. **Cross-Validation**:
   - The notebook includes cross-validation to validate model consistency across folds. The cross-validation scores will appear in the output as part of the execution flow.

### Usage and Results

Upon running the notebook, you should observe the following:
- A confusion matrix and classification report that highlights the model's accuracy, precision, recall, and F1-score.
- Visualizations of evaluation metrics (accuracy, precision, recall, F1-score) for easy interpretation of results.
- The model achieves high recall for the malignant class, which is essential for early and accurate medical diagnosis.

This project demonstrates the importance of data normalization and kernel methods in achieving reliable performance in medical image classification tasks. The high recall for malignant cases shows promise for real-world applications in medical diagnostics.
