# Bioactivity_Prediction_App

This is a web application for predicting the bioactivity of small molecules using machine learning models. The models were trained on publicly available datasets and are able to predict the activity of compounds against a variety of targets, including enzymes, receptors, and ion channels.

## Getting Started

To recreate this web app, you will need to have Python 3.6 or higher installed on your machine. You can clone the repository to your local machine using the following command:

```
git clone https://github.com/Janmejay-Vyas/Bioactivity_Prediction_App.git
```

Once you have cloned the repository, navigate to the project directory and install the required dependencies:

```
cd Bioactivity_Prediction_App
pip3 install -r requirements.txt
```
The machine learning model used in this web app will firstly have to be generated by successfully running the included Jupyter notebook [bioactivity_prediction_model.ipynb](./bioactivity_prediction_model.ipynb). Upon successfully running all code cells, a pickled model called bioactivity_model.pkl will be generated.

Finally, launch the app using

```
streamlit run app.py
```
## Using the app
When you first open the app, you will be presented with a form where you can input the SMILES string of a small molecule. Once you have entered a valid SMILES string, you can select a target from the dropdown menu and click the "Predict" button.

The app will then use a machine learning model to predict the bioactivity of the molecule against the selected target, and display the predicted activity score on the screen.
