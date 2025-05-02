# Neural Network Image Classification Project 🧠

This project implements a neural network using PyTorch to classify grayscale images from a custom dataset. The model is trained, validated, and tested with a focus on achieving high accuracy, and includes visualization of results using confusion matrices and performance metrics.

---

## 🌟 Overview

The project features a custom neural network designed for image classification tasks:
- **Dataset**: A custom dataset of grayscale images stored in a directory structure, loaded using a `CustomDataset` class.
- **Model Architecture**: A feedforward neural network with multiple fully connected layers, ReLU activation, and dropout for regularization.
- **Training**: Utilizes the Adam optimizer and CrossEntropyLoss over 20 epochs with a batch size of 32.
- **Evaluation**: Includes accuracy, precision, recall, F1 score, and a confusion matrix to assess model performance.
- **Visualization**: Plots training and validation metrics using Matplotlib and Seaborn.

The dataset is split into 70% training, 15% validation, and 15% test sets, with images normalized using a mean of 0.5 and standard deviation of 0.5.

---

## 📂 File Structure

- **NN.ipynb**: Jupyter Notebook containing the full implementation, including data loading, model definition, training, and evaluation.
- **train/**: Directory with the custom dataset (e.g., `C:/Users/Кирка/PycharmProjects/pythonProjectТNN/train`), organized into subdirectories for each class.

---

## 🚀 Setup Instructions

To set up and run this project locally, follow these steps:

1. **Prerequisites**:
   - Python 3.x
   - PyTorch
   - NumPy
   - Matplotlib
   - Seaborn
   - Scikit-learn
   - Pillow
   - torchvision

2. **Installation**:
   - Install required packages using pip:
     ```bash
     pip install torch numpy matplotlib seaborn scikit-learn pillow torchvision
     ```

3. **Dataset Preparation**:
   - Place your grayscale image dataset in the `train` directory (e.g., `C:/Users/Кирка/PycharmProjects/pythonProjectТNN/train`).
   - Ensure the directory contains subfolders, each named with a class label (e.g., `0`, `1`, etc.), containing the corresponding images.

4. **Run the Notebook**:
   - Open `NN.ipynb` in Jupyter Notebook or JupyterLab.
   - Update the `DATA_DIR` variable in the notebook to match your dataset path.
   - Execute all cells to train the model and view results.

---

## 🛠️ Usage

### Training the Model
- The model trains for 20 epochs with a learning rate of 0.001.
- Training and validation loss/accuracy are printed per epoch and stored for plotting.

### Evaluating the Model
- After training, the model is evaluated on the test set.
- A confusion matrix is generated to visualize true vs. predicted labels.
- Metrics (accuracy, precision, recall, F1 score) are calculated and displayed using a classification report.

### Viewing Results
- Run the plotting cell to see the confusion matrix.
- Check the final cell for detailed performance metrics.

---

## 🔮 Future Improvements

- **Hyperparameter Tuning**: Experiment with different learning rates, batch sizes, and dropout rates to optimize performance.
- **Model Architecture**: Add convolutional layers for better feature extraction with CNNs if applicable.
- **Data Augmentation**: Implement transforms like rotation or flipping to improve model robustness.
- **Cross-Validation**: Use k-fold cross-validation to ensure consistent performance across splits.
- **Export Model**: Save the trained model weights and provide a script for inference on new images.
- **GPU Support**: Enhance device detection and optimize for CUDA if available.

---

## 📜 License

This project is licensed under the MIT License - feel free to use and modify it as needed.