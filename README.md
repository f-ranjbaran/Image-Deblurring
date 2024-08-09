# Image Deblurring 

This repository contains the code and resources for the "Image Deblurring" project, which was developed as part of a Deep Learning course. The primary objective of this project is to build a model that can effectively remove blurring from images, using a dataset of artificially blurred images and their corresponding sharp versions.

## Project Overview

### Project Description

The goal of this project is to create a deep learning model capable of deblurring images. The dataset used for this purpose is derived from the CIFAR-10 dataset, which has been modified to include blurred images created using a Gaussian blur. The model is trained to reconstruct the original, sharp images from the blurred inputs.

### Key Features

- **Dataset Preparation**: The dataset is created by applying Gaussian blur to images from the CIFAR-10 dataset. The dataset is split into training, validation, and testing sets.
- **Model Architecture**: The project utilizes a convolutional neural network (CNN) designed to remove blur from images. The architecture includes both convolutional and deconvolutional layers.
- **Training**: The model is trained with specific callbacks, including learning rate reduction and model checkpointing, to enhance performance.

## Installation

To run this project locally, you need to have Python 3 and the following libraries installed:

- TensorFlow
- Keras
- NumPy
- OpenCV (for Gaussian blurring)
- Matplotlib
- Scikit-learn

You can install the required packages using pip:

```bash
pip install tensorflow keras numpy opencv-python matplotlib scikit-learn
```

## Usage

### Running the Code

1. Clone the repository:

   ```bash
   git clone https://github.com/f-ranjbaran/Image-Deblurring.git
   cd Image-Deblurring
   ```

2. Run the Jupyter Notebook:

   ```bash
   jupyter notebook Image_Deblurring.ipynb
   ```

3. Follow the steps in the notebook to load the data, create the model, train it, and evaluate its performance on the test set.

### Dataset Creation

The dataset is automatically generated using the `getDataset` function, which loads CIFAR-10 images, applies Gaussian blur, and adds a small amount of noise. This function should not be modified as it is crucial for maintaining the integrity of the dataset.

### Model Training

The model is trained using the noisy, blurred images as input and the original sharp images as the target. The notebook provides a detailed walkthrough of the training process, including data visualization and performance metrics.

## Results

The results of the model's performance, including training/validation loss and sample outputs, are displayed in the notebook. The model is expected to improve the sharpness of blurred images, though the effectiveness may vary based on the level of blurring and noise.

## Contributing

If you wish to contribute to this project, feel free to fork the repository and submit pull requests. Any improvements to the model architecture, training process, or dataset creation are welcome.

## Acknowledgments

- This project was developed as part of the Deep Learning course in Spring 2022.
- The CIFAR-10 dataset was used as the base for image processing.

---

For any questions or issues, please contact f.ranjbaran2020@gmail.com.
