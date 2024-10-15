# Health Assist

Health Assist is an intelligent healthcare prediction system designed to provide users with a preliminary diagnosis based on input symptoms. Using machine learning, this project identifies potential diseases and provides users with helpful information, such as precautions, medications, recommended diets, and workouts. This application aims to streamline the diagnostic process and promote healthier lifestyle decisions by offering accurate predictions and relevant advice.

### Features
**Symptom-Based Disease Prediction:** Users can input their symptoms, and the system predicts the most likely disease based on a trained Support Vector Classifier (SVC) model.

**Detailed Information:** After a prediction, the app provides disease descriptions, precautions to take, potential medications, dietary recommendations, and suitable workouts.

**User-Friendly Interface:** The Flask-based web application ensures ease of use with a simple, interactive UI that accepts symptoms and displays results promptly.

### Datasets Used
The project uses various datasets to deliver precise and actionable advice:

**Symptoms Dataset:** For mapping symptoms to diseases.

**Precautions Dataset:** Lists of precautions to take based on predicted diseases.

**Medications Dataset:** Suggested medications for each predicted disease.

**Diet Dataset:** Recommended diets tailored to the specific health condition.

**Workout Dataset:** Customized workout plans to complement recovery or health management.

### Machine Learning Model
The predictive engine of Health Assist is powered by a Support Vector Classifier (SVC) model, trained on a dataset of symptoms and corresponding diseases. The input data is processed into a binary vector format where symptoms are marked, and the model predicts the probable disease.

### How It Works
Users input their symptoms, separated by commas.
The model processes the input and predicts the disease.
**The app returns:**
-> Disease description

-> Precautionary steps

-> Suggested medications

-> Recommended diet plans
 
 -> Suggested workout routines

### Code Overview
**app.py:** Main Flask application for routing, user interaction, and displaying the results.

**Machine Learning Model:** A pre-trained model (svc.pkl) is loaded to perform predictions based on user input.

**Helper Functions:** Custom functions to fetch detailed descriptions, medications, diets, and workouts based on the disease predicted by the model.

### Setup Instructions
1. Clone this repository.
2. Install the required dependencies from the requirements.txt file.
3. Download or create the necessary datasets (symptoms, precautions, medications, diets, workout).
4. Run the Flask app:  python app.py

### Future Enhancements
* Adding more disease categories to increase prediction accuracy.
* Integrating real-time updates on medications and precautions from medical sources.
* Implementing a mobile-friendly version of the application.

### Project Link
You can find the complete project and further details here: https://medicine-recommendation-8mrz.onrender.com/
