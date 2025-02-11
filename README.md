

1. Problem Statement
The global COVID-19 pandemic emphasized the need for effective monitoring systems to ensure public safety. Many organizations and public spaces require individuals to wear face masks to minimize
 the spread of the virus. Monitoring compliance manually is time-consuming and inefficient. The problem is to build an automated system capable of detecting whether a person is wearing a mask or not
 using machine learning.


2. Project Overview
The Face Mask Detection System is an AI-powered solution that uses computer vision and deep learning to classify images of individuals as either "Wearing a Mask" or "Not Wearing a Mask." The project involves:
1)Backend: A CNN-based model trained on a dataset of images of individuals with and without masks.
2)Frontend: An interactive interface built using Gradio, allowing users to upload an image and get real-time predictions.
The project can be extended to real-time detection using webcams or integrated with CCTV systems for mask compliance monitoring.

3)
video Link

https://youtu.be/dNISjkFv084




4. Tech Stack
Backend
Programming Language: Python
Libraries:
TensorFlow/Keras for building the CNN model.
NumPy and Scikit-learn for preprocessing and splitting data.
OpenCV for image handling.
Dataset: Face Mask Dataset.
Frontend
Gradio: A Python-based library for building interactive GUIs for machine learning models.
Tools
Jupyter Notebook (or Google Colab) for training and testing the model.
Kaggle API for fetching the dataset.


5. Installation Guide
6. 
Step 1: Clone the Repository
bash
Copy code
git clone https://github.com/DeepVision/facemask-detection.git
cd facemask-detection
Step 2: Install Dependencies
bash
Copy code
pip install -r requirements.txt
Required libraries:

TensorFlow
NumPy
OpenCV
Gradio
Step 3: Download Dataset from Kaggle
Obtain your Kaggle API key (kaggle.json).
Place kaggle.json in the root directory of the project.
Run:
bash
Copy code
mkdir -p ~/.kaggle
cp kaggle.json ~/.kaggle/
chmod 600 ~/.kaggle/kaggle.json
kaggle datasets download -d omkargurav/face-mask-dataset
unzip face-mask-dataset.zip -d data/
Step 4: Run the Jupyter Notebook
Open the Jupyter Notebook in your IDE (or Google Colab).
Execute the cells one by one to train and evaluate the model.
Step 5: Launch the Gradio App
To test the model interactively, run the Gradio interface:

bash
Copy code
python app.py
Step 6: Upload Image and Get Prediction
Access the GUI via the provided localhost or public URL, upload an image, and view the prediction results.
