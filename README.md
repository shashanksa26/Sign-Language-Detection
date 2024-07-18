# Sign Language Detection

This project uses a pre-trained model to perform real-time sign language detection using a webcam. The model is trained to recognize specific sign language gestures such as "Hello", "Thank You", and "I am fine".

## Directory Structure

- `action.h5`: The pre-trained model on custom data file.
- `working_test.ipynb`: The Jupyter Notebook used for testing.
- `model_training.ipynb`: The Jupyter Notebook used for training the action.h5 model on Custom data collected through webcam.
- `demo.py`: The main script for running the real-time sign language detection demo.
- `MP_Data`: This folder contains the data in npy format for each category with 30 sets each, collected through webcam for model training.
- `requirements.txt`: Lists the Python dependencies required for the project.
- `README.md`: This file, which provides an overview of the project and instructions on how to use it.

Here's a step-by-step `README.md` guide for cloning and running the Sign Language Detection demo from GitHub:

## Setup Instructions

### Step 1: Clone the Repository

First, clone the repository from GitHub to your local machine:

```bash
git clone https://github.com/shashanksa26/Sign-Language-Detection.git
```

Navigate into the project directory:

```bash
cd Sign-Language-Detection
```

### Step 2: Install the Dependencies

Make sure you have Python installed on your machine. Then, install the required dependencies using pip:

```bash
pip install -r requirements.txt
```

### Step 3: Running the Demo

To run the real-time sign language detection demo using your webcam, execute the following command:

```bash
python demo.py
```

## Project Overview

This project leverages the MediaPipe library for detecting key points in the human body and a pre-trained TensorFlow model to recognize specific sign language gestures. The workflow includes:

1. Capturing video from the webcam.
2. Using MediaPipe to detect facial, pose, and hand landmarks.
3. Extracting key points from the detected landmarks.
4. Feeding the key points into a pre-trained model to predict the sign language gesture.
5. Displaying the predicted gesture on the video feed in real-time.

### Pre-trained Model

The pre-trained model `action.h5` is included in the root directory. It is trained to recognize the following gestures:

- Hello
- Thank You
- I am fine

### Jupyter Notebooks

- `model_training.ipynb`: Contains the code used to train the model. It provides a step-by-step explanation of the data processing, model training, and evaluation process.
- `working_test.ipynb`: Contains the code used to test the model.

### Python Scripts

- `demo.py`: Runs the real-time sign language detection demo. It captures video from the webcam, processes each frame to extract key points using MediaPipe, and uses the pre-trained model to predict and display the detected gesture.
```
