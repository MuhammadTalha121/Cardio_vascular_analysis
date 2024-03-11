# Cardio_vascular_analysis
Discover cardiovascular disease insights with our GitHub project. Datasets, analysis scripts, and predictive models aid in prevention and management. Join us to build a healthier future.
# Cardiovascular Disease Prediction Model Deployment

This project demonstrates how to deploy a classification model for predicting cardiovascular disease using Flask and joblib. The classification model is trained using TensorFlow/Keras and saved using joblib. The deployed Flask application provides an API endpoint for making predictions on new data.

## Requirements

- Python 3.x
- Flask
- joblib
- TensorFlow/Keras (for training the model)

## Installation

1. Clone the repository:

git clone https://github.com/MuhammadTalha121/Cardio_vascular_analysis.git



2. Navigate to the project directory:

cd Cardio_vascular_analysis

3. Install dependencies:

pip install -r requirements.txt


## Usage

1. Train the classification model using TensorFlow/Keras and save it using joblib. Modify the `train_model.py` script to load your dataset and train the model.

2. Deploy the Flask application by running the `app.py` script:

python app.py



3. Once the Flask application is running, you can make predictions by sending POST requests to the `/predict` endpoint with input data in JSON format. Example:

curl -X POST http://localhost:5000/predict -d '{"age": 50, "gender": 1, "chestpain": 0, "restingBP": 120, "serumcholestrol": 200, "fastingbloodsugar": 0, "restingrelectro": 1, "maxheartrate": 150, "exerciseangia": 0, "oldpeak": 1.5, "slope": 1, "noofmajorvessels": 0}' -H 'Content-Type: application/json'
