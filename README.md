# 🎵 Music Recommendation System

This project is developed as part of my **Machine Learning Internship at CodeAlpha**.  
It uses **unsupervised learning (K-Means Clustering)** along with **cosine similarity** to recommend similar songs based on audio features such as energy, valence, tempo, and more.

---

## 📌 Project Overview

This music recommendation system:
- Loads and preprocesses a dataset of songs
- Uses **K-Means Clustering** to group songs into clusters based on audio features
- Applies **PCA** to visualize clusters
- Recommends songs that are **sonically similar** to a selected song using **cosine similarity** within the same cluster

---

## 🔧 Technologies Used

- **Python**
- **Pandas**, **NumPy**
- **Scikit-learn** (StandardScaler, KMeans, PCA, Cosine Similarity)
- **Matplotlib**
- Dataset in CSV format (`data.csv`)

---

## 🎯 Features Used

The following audio features were used for clustering and similarity computation:
- `valence`
- `danceability`
- `energy`
- `tempo`
- `acousticness`
- `liveness`
- `speechiness`
- `instrumentalness`

---

## 📊 How It Works

1. **Load and preprocess** the data
2. Use the **Elbow Method** to find the optimal number of clusters (k)
3. Fit **K-Means clustering**
4. Visualize clusters using **PCA**
5. For a given input song:
   - Find its cluster
   - Compare it with other songs in the same cluster using **cosine similarity**
   - Return the top N most similar songs

---

## 🚀 How to Run the Project

1. Clone the repository:
   ```bash
   git clone https://github.com/BilawalMir/CodeAlpha_Music_Recommendation.git
   cd CodeAlpha_Music_Recommendation

2. Install the required Python libraries:
   ```pip install pandas numpy scikit-learn matplotlib

3. Make sure your dataset (data.csv) is in the same folder as the notebook/script.

4. Run the Python notebook or script.   

📦 Example

input_song = "Soul Junction"
recommended_songs = recommend_songs(input_song, df, num_recommendations=5)
print(recommended_songs)

📁 Repository Structure
CodeAlpha_Music_Recommendation/
├── data.csv
├── music_recommendation.ipynb
├── README.md

🙌 Acknowledgements
Thanks to @CodeAlpha for this exciting internship opportunity and real-world ML project.


📌 Author
Name: [Bilawal Mir]

Internship: Machine Learning Intern at CodeAlpha

GitHub: [https://github.com/BilawalMir]

LinkedIn: [www.linkedin.com/in/bilawal-mir-0b24911ba]