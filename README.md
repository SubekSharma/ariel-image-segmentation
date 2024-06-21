# Aerial Image Segmentation with PyTorch

This repository contains a project for performing aerial image segmentation using PyTorch. The notebook demonstrates how to preprocess data, build and train a U-Net segmentation model, and evaluate its performance.

## Table of Contents
- [Introduction](#introduction)
- [Dataset](#dataset)
- [U-Net Architecture](#u-net-architecture)
- [Setup](#setup)
- [Usage](#usage)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Introduction

Aerial image segmentation is a crucial task in various applications such as urban planning, agriculture, and disaster management. This project uses a Convolutional Neural Network (CNN), specifically a U-Net architecture, implemented in PyTorch to segment aerial images.

## Dataset

The dataset used in this project is available in the `Road_seg_dataset` repository. It includes aerial images and their corresponding segmentation masks. You can clone the dataset using the following command:

```bash
git clone https://github.com/parth1620/Road_seg_dataset.git
```

## U-Net Architecture

U-Net is a convolutional neural network architecture designed for biomedical image segmentation but has been widely adopted for various segmentation tasks. It consists of a contracting path to capture context and a symmetric expanding path that enables precise localization. The U-Net architecture ensures that the model can learn from a limited amount of data and produce high-quality segmentation results.

![image](https://github.com/SubekSharma/ariel-image-segmentation/assets/71229363/07ef0359-6157-4848-bb5f-6faf61d61b3f)


### Key Features of U-Net:
- **Contracting Path**: A series of convolutional and max-pooling layers to capture features and reduce spatial dimensions.
- **Bottleneck**: The deepest layer of the network which captures the most abstract representation of the input.
- **Expanding Path**: A series of up-convolutions and concatenations with high-resolution features from the contracting path to improve localization accuracy.

## Setup

To set up the project, follow these steps:

1. Clone this repository:
    ```bash
    git clone https://github.com/SubekSharma/ariel-image-segmentation.git
    ```

2. Navigate to the project directory:
    ```bash
    cd ariel-image-segmentation
    ```

3. Install the required packages:
    ```bash
    pip install -r requirements.txt
    ```

4. Clone the dataset repository:
    ```bash
    git clone https://github.com/parth1620/Road_seg_dataset.git
    ```

## Usage

1. Open the Jupyter notebook:
    ```bash
    jupyter notebook Aerial_Image_Segmentation_with_PyTorch.ipynb
    ```

2. Follow the instructions in the notebook to preprocess the data, build and train the model, and evaluate its performance.

## Results

The notebook includes various visualizations to show the segmentation results. Below are some sample outputs from the model:

![image](https://github.com/SubekSharma/ariel-image-segmentation/assets/71229363/a00a06b9-18fc-412a-ba2c-1c8ed604ba32)


## Contributing

Contributions are welcome! If you have any suggestions, bug reports, or improvements, please create an issue or submit a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

