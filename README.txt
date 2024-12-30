
# Health Prediction System

## Overview

The **Health Prediction System** is a machine learning-based web application that predicts the likelihood of **Heart Disease**, **Diabetes**, and **Parkinson's Disease** based on user inputs. The application uses pre-trained models to provide predictions in real-time. Users can enter their health-related data, and the system will output the probability of having one of the three diseases.

## Features

- Predicts the likelihood of **Heart Disease**.
- Predicts the likelihood of **Diabetes**.
- Predicts the likelihood of **Parkinson's Disease**.
- Built using **Streamlit** for the user interface and **Python** for backend processing.
- Models are pre-trained and hosted for quick access and predictions.

## Technologies Used

- **Python**: The programming language used to develop the backend of the application.
- **Streamlit**: A framework for creating web applications in Python with minimal code.
- **Scikit-learn**: A machine learning library used to create the predictive models.
- **Pickle**: Used to save and load pre-trained models.
- **Requests**: A Python library for making HTTP requests to fetch models from GitHub.
- **Streamlit-option-menu**: Provides a stylish sidebar menu for the application.

## Installation

To run this project locally, follow these steps:

### Prerequisites

Ensure you have **Python** installed on your machine. You can download it from [python.org](https://www.python.org/downloads/).

### 1. Clone the Repository

```bash
git clone https://github.com/MohammadErfanRashidi/Health-Prediction-System.git
cd Health-Prediction-System
```

### 2. Set up a Virtual Environment (Optional)

It is recommended to create a virtual environment to manage dependencies.

```bash
python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scriptsctivate`
```

### 3. Install Required Dependencies

Use `pip` to install the dependencies from `requirements.txt`:

```bash
pip install -r requirements.txt
```

This will install the necessary libraries such as Streamlit, Scikit-learn, and others required to run the application.

### 4. Run the Application

Once everything is installed, you can start the Streamlit app:

```bash
streamlit run app.py
```

This command will open the application in your default web browser, typically at `http://localhost:8501`.

## How It Works

1. The user enters their health data into the input fields.
2. The application uses pre-trained machine learning models to predict the likelihood of the following conditions:
    - **Heart Disease**
    - **Diabetes**
    - **Parkinson’s Disease**
3. The models are loaded from GitHub using `requests` and `pickle`.
4. Based on the input, the model returns a prediction, which is displayed in a user-friendly format.

## Models Used

- **Heart Disease Prediction Model**: This model predicts the likelihood of a person suffering from heart disease based on inputs such as age, cholesterol levels, blood pressure, etc.
- **Diabetes Prediction Model**: A model that predicts the likelihood of diabetes using inputs like body mass index, age, blood pressure, etc.
- **Parkinson's Disease Prediction Model**: This model predicts Parkinson's disease likelihood based on features extracted from a speech dataset.

All models are pre-trained and available as `.sav` files, which are loaded into the app for prediction.

## How to Access the Models

The models are hosted on GitHub and are accessed using the following raw URLs:

- **Heart Disease Model**: [Heart Disease Model](https://raw.githubusercontent.com/MohammadErfanRashidi/Disease-App/main/saved%20models/heart_disease_model.sav)
- **Diabetes Model**: [Diabetes Model](https://raw.githubusercontent.com/MohammadErfanRashidi/Disease-App/main/saved%20models/diabetes_model.sav)
- **Parkinson’s Model**: [Parkinson's Model](https://raw.githubusercontent.com/MohammadErfanRashidi/Disease-App/main/saved%20models/parkinsons_model.sav)

## Folder Structure

```
Health-Prediction-System/
│
├── app.py              # Main Streamlit app
├── models/             # Folder containing models (if stored locally)
├── requirements.txt    # Python dependencies
├── README.md           # Project overview
└── saved models/       # Folder containing pre-trained models
```

## Contributing

If you would like to contribute to this project, feel free to fork the repository and submit a pull request. Make sure to follow these steps:

1. Fork the repository.
2. Create a new branch for your changes.
3. Make your changes and test them.
4. Commit your changes and create a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
