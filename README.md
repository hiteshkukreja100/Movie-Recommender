# Movie-Recommender

This project is a movie recommendation system built with Python and Flask. It uses machine learning to recommend movies and predict movie ratings based on user preferences.

## Features

- **Recommend Movies:** Provides a list of recommended movies based on user ID and the number of recommendations needed.
- **Predict Movie Rating:** Predicts the rating a user would give to a specific movie.

## Requirements

- Python 3.x
- Flask
- Flask-Ngrok
- Requests
- Pandas
- NumPy
- TensorFlow
- TensorFlow Recommenders

## Installation

1. **Clone the Repository:**

    ```bash
    git clone https://github.com/hiteshkukreja100/Movie-Recommender.git
    cd movierecommender
    ```

2. **Install the Required Packages:**

    ```bash
    pip install -r requirements.txt
    ```

3. **Download and Set Up `ngrok`:**

    - Visit the [ngrok website](https://ngrok.com/) and sign up for a free account.
    - Download `ngrok` for your operating system and unzip it.

## Running the Application

1. **Start the Flask Application:**

    ```bash
    python app.py
    ```

    This will start the Flask server on `http://127.0.0.1:5000`.

2. **Start `ngrok`:**

    Open a new terminal window and navigate to the directory where `ngrok` is located. Run:

    ```bash
    ./ngrok http 5000
    ```

    `ngrok` will provide a public URL (e.g., `http://abcd1234.ngrok.io`) that you can use to access your Flask app.

## Using the API

### Get Movie Recommendations

To get movie recommendations, use the following endpoint:

```bash
curl "http://abcd1234.ngrok.io/recommend?user_id=100&top_n=3"
