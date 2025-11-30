# Car Price Prediction

This project helps you estimate the price of a used car based on its features.

## How it works

This project is a simple web application that uses a machine learning model to predict car prices. Here's a quick overview of how it's put together:

1.  **Data Collection**: We started with a dataset of used car listings from Quikr.
2.  **Data Cleaning**: The raw data was messy, so we cleaned it up. We removed things like "Ask for Price" and made sure all the data was in a consistent format.
3.  **Model Training**: We used the cleaned data to train a machine learning model. This model learned the relationships between a car's features (like its make, model, year, and mileage) and its price. We used a `RandomForestRegressor` model, which is good at this type of task.
4.  **Web Application**: We built a simple web application that lets you enter the details of a car you're interested in. The application then uses the trained model to predict the car's price.

## How to run this project

1.  Make sure you have Python and the required libraries installed. You can install the libraries by running:
    ```
    pip install -r api/requirements.txt
    ```
2.  Navigate to the `api` directory:
    ```
    cd api
    ```
3.  Run the Flask application:
    ```
    python main.py
    ```
4.  Open your web browser and go to `http://127.0.0.1:5000` to use the application.

## Files in this project

*   `quikr_car.csv`: The original, raw data we used.
*   `CarPrediction.ipynb`: A Jupyter Notebook that shows how we cleaned the data and trained the model.
*   `Cleaned_Car_data.xlsx`: The cleaned-up data that we used to train the model.
*   `api/`: A directory containing the web application.
    *   `main.py`: The main file for the web application.
    *   `RandomforestReg.pkl`: The trained machine learning model.
    *   `templates/home.html`: The HTML template for the web application's user interface.
    *   `requirements.txt`: A list of the Python libraries needed to run the web application.
