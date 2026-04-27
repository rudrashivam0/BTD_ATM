🧠 Brain Tumor Detection System (BTD_ATM)

🚀 Overview

This project is an AI-powered web application that detects brain tumors from MRI images using a deep learning model. It provides a simple interface where users can upload an image and get instant predictions.

⸻

🎯 Problem Statement

Early detection of brain tumors is critical but often requires expert radiologists.
This project aims to assist in preliminary diagnosis using machine learning.

⸻

🧩 Features

* 🖼️ Upload MRI scan images
* 🤖 Predict tumor presence using CNN model
* ⚡ Fast and real-time inference
* 🌐 Web-based interface (Flask)
* 📊 Clean UI with structured sections

⸻

🏗️ Tech Stack

🔹 Backend

* Python
* Flask

🔹 Machine Learning

* Convolutional Neural Network (CNN)
* Trained on Brain MRI dataset
* Model file: .h5

🔹 Frontend

* HTML, CSS
* Jinja Templates

⸻

🧠 Model Details

* Architecture: CNN with attention mechanism
* Input: MRI brain scan image
* Output: Tumor classification

Classes:

* Glioma
* Meningioma
* Pituitary
* No Tumor

📁 Project Structure
BTD_ATM/
│── main.py
│── templates/
│   ├── index.html
│   ├── Sections/
│── uploads/
│── static/ (if added later)
│── .gitignore
│── README.md


⚙️ Installation & Setup

1️⃣ Clone the repository
git clone https://github.com/rudrashivam0/BTD_ATM.git
cd BTD_ATM

2️⃣ Install dependencies
pip install -r requirements.txt

3️⃣ Run the application
python main.py

4️⃣ Open in browser
http://127.0.0.1:5000

📦 Model Download
Due to GitHub size limits, the trained model is not included.
👉 Download model from:
(https://drive.google.com/file/d/1P2QSn5uXiPP_kH1U8xzH4EHA-CIs3CiD/view?usp=drive_link)

⚠️ Limitations

* Not a replacement for medical diagnosis
* Accuracy depends on dataset quality
* Works best on similar MRI formats

📜 License

This project is for educational purposes.

⸻

👨‍💻 Author

Shivam Sharma

* GitHub: https://github.com/rudrashivam0
