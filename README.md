# 🎬 CineMood AI: Personalized Movie Recommendation System

CineMood AI is an AI-based movie recommendation system that suggests movies based on user ratings, mood, preferred genre, and similarity with other users. The project uses collaborative filtering with cosine similarity and a custom CineScore ranking system to generate personalized movie recommendations.

---

## 📌 Project Overview

This project was developed as part of an Artificial Intelligence and Machine Learning internship task.

The main goal of the project is to build a movie recommendation system that recommends movies based on user interests and rating patterns. To make the project more creative and interactive, CineMood AI includes mood-based recommendation, Movie Twin detection, Movie Personality tagging, CineScore ranking, explainable recommendations, cold-start recommendation, and an interactive Gradio interface.

---

## ✨ Features

* User-based collaborative filtering
* Mood-based movie recommendation
* Preferred genre filtering
* Movie Twin feature
* Movie Personality detection
* CineScore ranking system
* Explainable recommendation reasons
* Cold-start recommendation for new users
* Weekend watchlist generator
* Data visualizations
* Interactive Gradio web interface

---

## 📂 Dataset

The project uses the **MovieLens Latest Small Dataset**.

Files used:

* `movies.csv`
* `ratings.csv`

The dataset contains movie information, genres, user IDs, movie IDs, ratings, and timestamps.

---

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Scikit-learn
* Google Colab
* Gradio

---

## 🧠 Algorithm Used

The system uses **user-based collaborative filtering**.

A user-movie rating matrix is created where:

* Rows represent users
* Columns represent movies
* Values represent ratings

Missing ratings are filled with zero. Then, cosine similarity is calculated between users to find users with similar movie preferences. Movies liked by similar users are recommended to the selected user.

---

## 🔥 CineScore Formula

CineScore is a custom ranking score used to improve recommendation quality.

CineScore is calculated using:

* 50% similar user rating score
* 30% average movie rating
* 20% movie popularity score

This helps recommend movies that are not only similar to user taste but also highly rated and popular.

---

## 🎭 Mood-Based Recommendation

The system maps user mood to suitable movie genres.

| Mood        | Recommended Genres           |
| ----------- | ---------------------------- |
| Happy       | Comedy, Animation, Adventure |
| Sad         | Drama, Romance               |
| Stressed    | Comedy, Fantasy, Family      |
| Romantic    | Romance, Drama               |
| Adventurous | Action, Adventure, Sci-Fi    |
| Bored       | Thriller, Mystery, Crime     |

---

## 👥 Movie Twin Feature

The Movie Twin feature finds another user with similar movie taste using cosine similarity. It displays the most similar user and the taste similarity percentage.

---

## 🧩 Movie Personality Feature

Based on the user’s highly rated movies, the system detects the user’s movie personality.

Examples:

* The Sci-Fi Explorer
* The Action Hunter
* The Romantic Dreamer
* The Thriller Detective
* The Comfort Viewer
* The Deep Thinker
* The Adventure Seeker

---

## 🆕 Cold-Start Recommendation

If the user is new or the user ID is invalid, the system recommends movies based on:

* Mood
* Preferred genre
* Average movie rating
* Movie popularity

This helps solve the cold-start problem in recommendation systems.

---

## 🍿 Weekend Watchlist

The system generates a weekend watchlist from the recommended movies.

Example:

* Friday Night
* Saturday Afternoon
* Saturday Night
* Sunday Evening
* Bonus Pick

---

## 📊 Visualizations

The project includes the following charts:

* Top 10 most rated movies
* Rating distribution
* Top 10 movie genres
* CineScore comparison chart

---

## 🖥️ Interface

An interactive web interface was built using **Gradio**.

Users can enter:

* User ID
* Current mood
* Preferred genre
* Number of recommendations

The interface displays:

* Recommended movies
* Movie Personality
* Movie Twin
* CineScore
* Recommendation explanation
* Weekend watchlist
* Recommendation table

---

## 📁 Project Structure

```text
CineMood-AI/
│
├── dataset/
│   ├── movies.csv
│   └── ratings.csv
│
├── notebook/
│   └── CineMood_AI.ipynb
│
├── outputs/
│   ├── screenshots/
│   └── cinemood_ai_recommendations.csv
│
├── report/
│   └── CineMood_AI_Report.pdf
│
├── README.md
└── requirements.txt
```

---

## 🚀 How to Run the Project

### 1. Clone the repository

```bash
git clone https://github.com/your-username/CineMood-AI.git
```

### 2. Open the project folder

```bash
cd CineMood-AI
```

### 3. Install required libraries

```bash
pip install -r requirements.txt
```

### 4. Open the notebook

Open `CineMood_AI.ipynb` in Google Colab or Jupyter Notebook.

### 5. Run all cells

Run the notebook cells step by step to load the dataset, perform analysis, generate recommendations, and launch the Gradio interface.

---

## 📌 Sample Output

```text
User ID: 25
Mood: Adventurous
Preferred Genre: Sci-Fi

Movie Personality: The Sci-Fi Explorer
Movie Twin: User 118
Taste Similarity: 84%

Top Recommendations:
1. The Matrix
2. Star Wars
3. Jurassic Park
4. Terminator 2
5. Men in Black
```

---

## 📄 Project Report

The project report is available in the `report/` folder.

It includes:

* Introduction
* Objective
* Dataset description
* Methodology
* Features
* Visualizations
* Interface screenshots
* Conclusion

---

## ✅ Conclusion

CineMood AI successfully demonstrates a personalized movie recommendation system using collaborative filtering and cosine similarity. The system recommends movies based on user rating patterns and improves personalization using mood, genre preference, CineScore, Movie Twin, Movie Personality, and explainable recommendations.

The project also includes an interactive Gradio interface, making it simple and user-friendly for users to generate movie recommendations.

---

## 👩‍💻 Developed By

**Petrisha V**

B.Tech CSE - Data Science
CMR University, Bengaluru
