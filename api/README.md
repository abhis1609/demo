
# Real-Time Face Mask Detection

This repository contains code and resources for real-time face mask detection using computer vision techniques. The goal is to detect whether a person in a video stream is wearing a face mask or not. The project utilizes deep learning models to achieve accurate and efficient mask detection.

## Table of Contents
- [Introduction](#introduction)
- [Installation](#installation)
- [Usage](#usage)
- [Model Training](#model-training)
- [Contributing](#contributing)
- [License](#license)

## Introduction
The real-time face mask detection system aims to promote public health and safety by automatically detecting if individuals are wearing face masks. It can be deployed in various scenarios, such as airports, hospitals, offices, and public spaces, to monitor compliance with mask-wearing guidelines.

The system leverages computer vision techniques and deep learning models to analyze video streams and detect faces. It then determines if a detected face is wearing a mask or not. The detection process is performed in real-time, enabling quick and proactive responses in case of non-compliance.

## Installation
To install the necessary dependencies, follow these steps:

1. Clone this repository:
   ```
   git clone git clone https://github.com/your-username/real-time-face-mask-detection.git
   ```

2. Navigate to the project directory:
   ```
   cd real-time-face-mask-detection
   ```

3. Install the required packages:
   ```
   pip install -r requirements.txt
   ```

## Usage
To use the real-time face mask detection system, follow these steps:

1. Launch the application:
   ```
   python app.py
   ```

2. The system will access your webcam and start analyzing the video stream in real-time.

3. The output will display bounding boxes around detected faces, along with labels indicating whether masks are being worn or not.

4. To quit the application, press 'Q' on your keyboard.

## Model Training
The project includes a pre-trained model, but if you wish to train your own model or fine-tune the existing one, follow these steps:

1. Prepare your dataset:
   - Create a dataset of images with annotations indicating whether each face is wearing a mask or not.
   - Organize the dataset into two classes: "with_mask" and "without_mask".
   - Split the dataset into training and validation sets.

2. Configure training parameters:
   - Open the `train.py` file and modify the parameters according to your needs.
   - Set the dataset path, model architecture, batch size, number of epochs, etc.

3. Train the model:
   - Run the following command to start the training process:
     ```
     python train.py
     ```

4. Evaluate the trained model:
   - Once training is complete, you can evaluate the model's performance on the validation set:
     ```
     python evaluate.py
     ```

5. Save the trained model:
   - After training and evaluation, save the trained model's weights for future use:
     ```python
     model.save_weights('trained_model.h5')
     ```

## Contributing
Contributions to this project are welcome. If you find any issues or have suggestions for improvement, please open an issue or submit a pull request.

## License
This project is licensed under the [MIT License](LICENSE). Feel free to use, modify, or distribute the code for your purposes.
