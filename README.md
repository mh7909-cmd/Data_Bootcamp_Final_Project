# Spotify Popularity Predictor: A Data Science Project
**Data Bootcamp Final Project | Machine Learning Portfolio**

## What this project is about
We analyzed the Spotify music library to figure out what actually makes a song popular today. As the music industry moves away from human gatekeepers and toward algorithmic decision-making, we wanted to see if technical audio features like loudness and energy could predict a song's success. By looking at a dataset of over 32,000 tracks, we built a series of models to find the hidden patterns in digital music.

## How we organized the work
The project is split into two parts that follow our research from start to finish.

### [Part 1: Exploratory Data Analysis](file:///Users/mayankhinduja/Desktop/Spotify%20Final%20Project/1_EDA_Analysis.ipynb)
In the first part of the project, we focused on cleaning the data and looking for initial trends. 
- **Data Source**: We used the 30,000 Spotify Songs dataset from the Spotify Web API.
- **Data Cleaning**: We removed duplicates and fixed missing values to make sure our results were accurate.
- **Time Trends**: We looked at release years and months to see if certain times of the year produce more hits.
- **Audio Features**: We checked how metrics like energy and danceability correlate with popularity.

### [Part 2: Predictive Modeling](file:///Users/mayankhinduja/Desktop/Spotify%20Final%20Project/2_Predictive_Modeling.ipynb)
After we understood the data, we moved on to building models that can estimate a song's popularity score.
- **Baseline Models**: We started with simple Linear and Ridge regressions to set a benchmark.
- **Non-Linear Relationships**: We used polynomial features to see if the connections between audio metrics were more complex than a straight line.
- **Ensemble Models**: We trained Random Forest and XGBoost models to improve our accuracy.
- **Final Optimization**: We combined our best models into a Stacking Ensemble to get the best possible predictions.
- **Vibe Check**: We used K-Means clustering to group songs into different "vibes" based on their sound.
- **Spotting Hits**: We used Logistic Regression to see if we could identify tracks with viral potential early on.

## Our Approach
We handled the data using an automated pipeline in Scikit-Learn.
- **Scaling**: We used a robust scaling method to handle songs that had extreme values in loudness.
- **Feature Selection**: We identified which audio features were the most important for the models.
- **Validation**: We used cross-validation and looked at learning curves to make sure our models weren't just memorizing the data.

## What we found
Our results show that popularity isn't just random luck. 
- **The Stacking Winner**: Our Stacking Ensemble performed the best, proving that combining different types of models is the way to go.
- **The Loudness War**: Loudness is the single biggest predictor of popularity. It seems the algorithm really does favor music that is loud and energetic.
- **Vocals Matter**: We found a strong negative correlation with instrumental music. Listeners (and the algorithm) still prefer the sound of a human voice.
- **Engagement**: The data suggests that Spotify favors music that keeps people listening for longer stretches of time.

## Tools we used
- **Python**: The core language for our analysis.
- **Libraries**: Pandas, NumPy, Scikit-Learn, XGBoost, SHAP and Scipy.
- **Graphics**: Matplotlib, Seaborn and Plotly.

