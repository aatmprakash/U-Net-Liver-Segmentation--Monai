# U-Net Liver Segmentation - MONAI

This repository contains the implementation of a U-Net model for segmenting liver regions in medical images using the MONAI (Medical Open Network for AI) framework. The U-Net architecture, combined with the MONAI toolkit, enables accurate and efficient liver segmentation, which is crucial for various medical imaging applications.

## Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Model Architecture](#model-architecture)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Introduction

Liver segmentation plays a vital role in medical imaging analysis, assisting in diagnosis, treatment planning, and surgical interventions. The U-Net model, combined with the MONAI framework, provides a powerful solution for automating liver segmentation tasks.

This project aims to develop a deep learning model using the U-Net architecture and the MONAI toolkit to accurately segment liver regions in medical images. The U-Net architecture, with its symmetric encoder-decoder structure, allows for precise localization and segmentation of the liver, while the MONAI framework provides a comprehensive set of tools and utilities specifically designed for medical imaging tasks.

## Dataset

The dataset used for training and evaluation is not included in this repository due to privacy and licensing restrictions. However, the code provided assumes that the dataset follows a specific directory structure. The dataset should consist of medical images and their corresponding ground truth segmentation masks for liver regions.

Ensure that the dataset is organized into separate folders for images and masks. It is crucial to align the image and mask pairs correctly.

## Model Architecture

The U-Net model is implemented using the MONAI framework, which provides high-level abstractions and utilities for medical imaging tasks. The U-Net architecture consists of an encoder path that captures contextual information and a decoder path that recovers spatial details. Skip connections are used to bridge the gap between the encoder and decoder, facilitating the fusion of low-level and high-level features.

The combination of the U-Net architecture and the MONAI framework enables efficient and accurate liver segmentation from medical images.

## Installation

To use this repository, follow these steps:

1. Clone the repository:

   ```
   git clone https://github.com/aatmprakash/U-Net-Liver-Segmentation--Monai.git
   ```

2. Install the required dependencies using `pip`:

   ```
   pip install -r requirements.txt
   ```

3. Organize your dataset according to the provided directory structure, as described in the Dataset section.

## Usage

Before running the code, ensure that you have installed the required dependencies and organized your dataset correctly.

To train the U-Net model, run the following command:

```
python train.py
```

The model will begin training using the specified dataset and hyperparameters. The trained model checkpoints will be saved for future use.

To evaluate the model on the test dataset, run the following command:

```
python evaluate.py --model saved_models/unet.pth
```

Replace `unet.pth` with the appropriate saved model checkpoint file.

## Results

The evaluation script will provide quantitative metrics such as dice coefficient, sensitivity, and specificity to assess the performance of the trained U-Net model on the test dataset. Additionally, visualizations of the predicted liver segmentations can be generated for qualitative analysis.

The results obtained from the evaluation can help in understanding the model's accuracy and robustness in segmenting liver regions in medical images.

## Contributing

Contributions to this repository are welcome. If you encounter any issues or have suggestions for improvements, please open an issue or submit a pull request. Collaboration and feedback from the community can help enhance the

 model's performance and make it more versatile for liver segmentation tasks.

## License

This project is licensed under the [MIT License](LICENSE). You are free to modify, distribute, and use the code for both non-commercial and commercial purposes, with proper attribution to the original authors.
