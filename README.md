Fruit Image Classifier using CNN, VGG16 & ResNet-50

Overview
This project implements a fruit image classifier using deep learning models:
1.	Custom CNN (baseline)
2.	VGG16 (transfer learning)
3.	ResNet-50 (transfer learning)

The classifier is trained on the Fruits360 dataset (10-class subset from Kaggle) and can predict fruit types from uploaded images.
A Streamlit web app is included to demonstrate real-time predictions.

link: Kaggle fruit dataset link

Installation

Clone this repository and install dependencies:

you can run it on you cmd(command prompt):

git clone GitHub link here
cd fruit-classifier

# Create virtual environment (optional)
python -m venv venv
source venv/bin/activate   # on Linux/Mac
venv\Scripts\activate      # on Windows

# Install requirements
pip install -r requirements.txt

#Running the Web App (Streamlit)

NOTE: BEFOE RUNNING APP Make sure you have the trained model (best_vgg16.keras or best_cnn.keras) and class_indices.json inside the project folder.

#Run the app:
streamlit run fruitapp.py

Steps:

1.	Upload a fruit image (.jpg/.png).

2. The app will:

Display the uploaded image.

Predict fruit class using trained model.

Show class name + confidence score.

Training Models (Google Colab)

⦁	Open the notebook: Fruit_Classifier.ipynb in Google Colab.
⦁	Mount Kaggle or upload the dataset.
⦁	Run all cells to:
 	1.Train Custom CNN
        2.Train & fine-tune VGG16
        3.Train & fine-tune ResNet-50
⦁	Best models will be saved under /models as .keras files.

Results
⦁	CNN & VGG16 achieved perfect classification on the 10-class subset.
⦁	Streamlit app successfully classified external fruit images.

Future Work

Train on full Fruits360 dataset (100+ classes).

Deploy Streamlit app to Heroku/Streamlit Cloud.

Explore CLIP or other zero-shot models for unseen fruits.

Author

Name: Shaik Neelofar

Institute: IIT Mandi

Track: Data Science & Machine Learning
