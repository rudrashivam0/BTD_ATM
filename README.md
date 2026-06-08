## Brain Tumor Detection using MRI Scans — BTD_ATM
Brain tumors are among the most critical neurological conditions where early detection can dramatically change patient outcomes. The challenge, however, is that reading MRI scans accurately demands trained radiologists and a lot of time — two things that aren't always available. This project is an attempt to bridge that gap using deep learning.
BTD_ATM is a CNN-based web application that analyzes brain MRI images and classifies them into one of four categories: Glioma, Meningioma, Pituitary tumor, or No Tumor. It's built as a practical tool for educational and research use, wrapped in a simple Flask web interface that anyone can run locally.

## Why This Exists
The idea behind this project is straightforward: if a convolutional neural network can learn to distinguish tumor types from thousands of MRI images, it can serve as a useful first-pass screening tool. It won't replace a radiologist — and it's not trying to. But it can flag cases that warrant closer attention, assist in teaching environments, or simply demonstrate how machine learning is being applied in medical imaging.

## What It Can Do

- Accept MRI brain scan images through a browser-based upload interface
- Run the image through a trained CNN model in real time
- Return a classification result with one of four possible outputs:

- Glioma — a tumor that starts in the glial cells of the brain or spine
- Meningioma — a tumor arising from the meninges, the membranes surrounding the brain
- Pituitary — a tumor in the pituitary gland at the base of the brain
- No Tumor — no detectable tumor present in the scan


## Tech Stack
## Backend

- Python 3
- Flask — handles routing, file uploads, and serving predictions

## Machine Learning

- TensorFlow / Keras — model training and inference
- CNN with an attention mechanism — helps the model focus on diagnostically relevant regions of the MRI
- Trained on a publicly available Brain MRI dataset
- Model saved in .h5 format

## Frontend

- HTML and CSS with Jinja2 templating
- Clean, minimal layout built for quick interaction

## Model Architecture
The core of the project is a Convolutional Neural Network designed specifically for image classification tasks. What makes this model a bit more interesting than a standard CNN is the addition of an attention mechanism — a layer that learns to assign higher importance to specific spatial regions in the image. In practice, this means the model isn't just looking at the whole scan uniformly; it's learning to pay more attention to areas that are more likely to indicate pathology.

Input to the model is a preprocessed MRI image, and the output is a probability distribution across the four classes. The class with the highest probability is returned as the prediction.

## Project Structure

```text
BTD_ATM/
├── main.py                  # Flask application
├── templates/
│   ├── index.html           # Main UI page
│   └── Sections/            # Reusable Jinja2 components
├── uploads/                 # Uploaded MRI images
├── static/                  # CSS, JS, Images
├── .gitignore               # Git ignored files
└── README.md                # Project documentation
```

## Download the model

The trained model file is too large to host on GitHub directly. Download it from the link below and place it in the root project directory:
Download model from Google Drive
After downloading, the file should be at: https://drive.google.com/file/d/1P2QSn5uXiPP_kH1U8xzH4EHA-CIs3CiD/view?usp=drive_link

```
BTD_ATM/
└── model.h5    ← place it here
```
## Author

Built by Shivam Sharma

GitHub: github.com/rudrashivam0
