# Cervical Cancer Prediction Website

## Overview
This project provides a web-based application for predicting the likelihood of cervical cancer in patients. It uses a trained Random Forest model to analyze user-provided medical data and return predictions alongside probabilities.

## Features
- Predict the likelihood of cervical cancer based on patient medical data.
- Display prediction results clearly: "Has Cancer" or "Does Not Have Cancer".
- Provide probabilities for each prediction for better interpretability.
- User-friendly interface for easy input of patient data.

## Technologies Used
- **Python** for backend development and machine learning model.
- **Flask** for creating the web application.
- **Scikit-learn** for training and using the Random Forest model.
- **HTML/CSS** for the frontend interface.
- **Joblib** for saving and loading the trained model.

## Dataset
The model was trained on a cervical cancer dataset, which includes features such as:
- Age
- Number of sexual partners
- First sexual intercourse age
- Number of pregnancies
- Smoking history
- Hormonal contraceptives usage
- STD history

## Installation
To set up the project locally, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/cervical-cancer-prediction.git
   cd cervical-cancer-prediction
   ```

2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the Flask app:
   ```bash
   python app.py
   ```

4. Open your browser and go to `http://127.0.0.1:5000` to access the web application.

## Usage
1. Input patient data into the provided fields on the website.
2. Click the **Predict** button.
3. View the prediction results, including whether the patient is likely to have cervical cancer and the probabilities for each outcome.

## File Structure
```
├── app.py                  # Main Flask application
├── model.pkl               # Trained Random Forest model
├── scaler.pkl              # StandardScaler used for data preprocessing
├── templates/              # HTML files for the web interface
│   ├── index.html          # Main webpage
├── static/                 # CSS and JS files
│   ├── style.css           # Styling for the webpage
├── requirements.txt        # Python dependencies
├── README.md               # Project documentation
```

## API Endpoints
- **`GET /`**: Renders the homepage.
- **`POST /predict`**: Accepts patient data and returns prediction results.

## Model Details
- **Algorithm**: Random Forest Classifier
- **Accuracy**: 99.1% on the test dataset
- **Metrics**:
  - Precision: 0.89 for class 1 (Has Cancer)
  - Recall: 0.80 for class 1
  - F1-Score: 0.84 for class 1

## Future Enhancements
- Add authentication for secure access.
- Enable batch predictions for multiple patients at once.
- Integrate visualization tools for better interpretability.

## Contributing
Contributions are welcome! Please follow these steps:
1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch-name`).
3. Commit your changes (`git commit -m 'Add some feature'`).
4. Push to the branch (`git push origin feature-branch-name`).
5. Open a pull request.

## License
This project is licensed under the MIT License. See the LICENSE file for details.


## Contact
For questions or suggestions, feel free to reach out:
- **Email**: A01174639@tec.mx
- **LinkedIn**: [Leonardo Andrade ](www.linkedin.com/in/leonardoandradeflores1)

