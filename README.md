# Clustering-and-suggesting-Spotify-music

10_Clustering_Algorithms.ipynb includes 10 methods for unsupervised clustering and their visualisations in 2D.

Methods used: AffinityPropagation, AgglomerativeClustering, Birch, DBSCAN, KMeans, MiniBatchKMeans, MeanShift, OPTICS, SpectralClustering, GaussianMixture

Spotify_Music_Recommendation_System_with_Clustering_between_genres_and_songs_with_preliminary_EDA.ipynb contains:

An Exploratory Data Analysis on the genres of music dataset with 21 feeatures: 'danceability', 'energy', 'key', 'loudness', 'mode', 'speechiness',
       'acousticness', 'instrumentalness', 'liveness', 'valence', 'tempo',
       'type', 'id', 'uri', 'track_href', 'analysis_url', 'duration_ms',
       'time_signature', 'genre', 'song_name', 'Unnamed: 0', 'title'
       
We display the correlation heatmap, the data in a pairplot, the histogram of all features, the scatter, regression, KDE and hex boxes between valence and loudness. Then we display the jointplot, Hex between acousticness and danceability. Also the jointplot between mode and instrumentalnes; the relation between energy and loudness(db) with regplot.

Then we enter the modelling phase: first a modelling on the genres of musics with a PCA with 2 components to visualize spacially the different genres; then a NeighborhoodComponentsAnalysis followed by a KNeighborsClassifier to see how well we can predict the genre of a music based on the other features.

Finally I clustered song names and suggest new ones related to a user's proposal of song using NearestCentroid. For example the song 'Still D.R.E.' suggested 'BOP'
