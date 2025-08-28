# Spotify_Playlist_Recommender_03 CaseCraft Analytics Project 3

## 🎧 Overview  
This project builds a content-based Spotify playlist recommender using audio features. It simulates a dataset of 500 tracks and applies cosine similarity to suggest songs with similar acoustic profiles.

## 🎯 Objective  
To recommend tracks within a playlist based on audio characteristics—mimicking Spotify’s “More Like This” feature.

## 📊 Dataset & Features  
- 500 synthetic tracks  
- Metadata: track name, artist, genre  
- Audio features: danceability, energy, valence, tempo, acousticness, instrumentalness, duration  

## 🧪 Feature Engineering  
- Selected key audio features  
- Scaled using `StandardScaler` for cosine similarity  
- Correlation heatmap reveals weak inter-feature dependencies

## 📈 Visual Explorations  
- Boxplot: Danceability by genre  
- Scatterplot: Energy vs Valence (emotional tone)  
- Histogram: Tempo distribution  
- Genre frequency bar chart  
- Acousticness vs Instrumentalness scatterplot

## 🤖 Recommender Logic  
- Cosine similarity computed across scaled audio features  
- For a given track, top 5 most similar tracks are returned  
- Recommendations span genres and artists, focusing purely on acoustic similarity

## 🧠 Key Insights  
1. **Genre-Agnostic Suggestions**: Recommendations are based on sound profile, not genre or artist  
2. **Feature Clusters**: Energy and valence show moderate correlation—useful for mood-based playlists  
3. **Tempo Trends**: Most tracks fall within 120–140 BPM, aligning with mainstream music  
4. **Ambient vs Instrumental**: Scatterplot reveals genre tendencies in acousticness and instrumentalness  
5. **Scalability**: Logic can be extended to real Spotify datasets via API integration

## ✅ Final Conclusion  
This recommender system demonstrates how audio features alone can drive personalized playlist expansion. By leveraging cosine similarity, it offers genre-flexible, mood-aware suggestions that enhance user engagement and discovery.