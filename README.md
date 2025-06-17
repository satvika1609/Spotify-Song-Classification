# Spotify Song Classifier

This project is a web application that allows users to enter a song name and predicts whether the song is *liked* or *not liked*. It uses the Spotify Web API to extract audio features and a machine learning classification model trained on a labeled dataset.


## Features

- Input any song name
- Fetches audio features from Spotify such as:
  - Danceability
  - Energy
  - Valence
  - Tempo
  - Acousticness and more
- Uses a trained machine learning model to classify the song
- Simple frontend built with HTML and CSS
- Backend powered by Flask


## Tech Stack

- Frontend: HTML, CSS
- Backend: Python (Flask)
- Machine Learning: scikit-learn (model trained and saved using `pickle`)
- API: Spotify Web API for audio feature extraction


## Setup Instructions

1. **Clone the repository**
   git clone https://github.com/satvika1609/Spotify-Song-Classification.git
   cd spotify-song-classifier

2. **Install dependencies**

   pip install -r requirements.txt

3. **Set up Spotify API credentials**

   * Go to [Spotify Developer Dashboard](https://developer.spotify.com/dashboard/)
   * Create an app and get your Client ID and Client Secret
   * Set them as environment variables or directly in your script:

     SPOTIPY_CLIENT_ID = 'your-client-id'
     SPOTIPY_CLIENT_SECRET = 'your-client-secret'

4. **Run the application**

   python app.py
   

5. **Access the app**
   Open your browser and go to `http://localhost:5000`


## Model Details

* The model is trained on Spotify audio features
* It performs binary classification: Liked (1) or Not Liked (0)
* Algorithms such as Logistic Regression or Random Forest may have been used
* The final model is serialized with `pickle` and integrated with Flask


## Acknowledgements

* [Spotify Web API](https://developer.spotify.com/)
* [Flask](https://flask.palletsprojects.com/)
* [scikit-learn](https://scikit-learn.org/)
