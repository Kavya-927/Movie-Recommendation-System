# 🎬 Movie Recommendation System

A content-based **Movie Recommendation System** built using Python and Machine Learning. The system recommends movies similar to a movie selected by the user based on movie metadata such as genres, keywords, cast, crew, and overview.

The project also includes an interactive **Streamlit web application** where users can select a movie and receive recommendations instantly.

---

## 🚀 Features

* 🎥 Search/select movies from the dataset
* 🤖 Content-based movie recommendations
* 🔍 Calculates similarity between movies
* 🎭 Uses movie metadata such as genres, keywords, cast, crew, and overview
* ⚡ Fast recommendation using cosine similarity
* 🌐 Interactive Streamlit web interface
* 📊 Data preprocessing and feature engineering using Pandas

---

## 🛠️ Technologies Used

* **Python**
* **Pandas** — Data manipulation and preprocessing
* **NumPy** — Numerical operations
* **Scikit-learn** — Machine learning and cosine similarity
* **NLTK / Python NLP techniques** — Text preprocessing
* **Streamlit** — Web application
* **Jupyter Notebook** — Development and experimentation

---

## 📂 Project Structure

```text
Movie-Recommendation-System/
│
├── app.py
├── movie_recommender.ipynb
│
├── tmdb_5000_movies.csv
├── tmdb_5000_credits.csv
│
├── requirements.txt
├── README.md
└── .gitignore
```

---

## 📊 Dataset

This project uses the **TMDB 5000 Movie Dataset**, consisting of movie information and credits.

The dataset contains information such as:

* Movie title
* Genres
* Keywords
* Overview
* Cast
* Crew
* Production companies
* Release information
* Popularity
* Vote count
* Vote average

---

## ⚙️ How It Works

The recommendation system follows these steps:

### 1. Data Collection

Two datasets are used:

* `tmdb_5000_movies.csv`
* `tmdb_5000_credits.csv`

### 2. Data Preprocessing

The movie and credits datasets are merged using the movie ID.

Relevant features are extracted from the dataset, including:

* Genres
* Keywords
* Cast
* Crew
* Overview

### 3. Feature Engineering

The extracted information is combined into a single feature representation for each movie.

Text preprocessing is performed to make the movie features suitable for similarity calculation.

### 4. Vectorization

Movie features are converted into numerical vectors using **CountVectorizer**.

### 5. Similarity Calculation

**Cosine Similarity** is used to calculate how similar two movies are.

The similarity score can be represented as:

```text
Cosine Similarity = (A · B) / (||A|| × ||B||)
```

Movies with higher similarity scores are considered more similar.

### 6. Recommendation

When a user selects a movie, the system:

1. Finds the selected movie.
2. Calculates its similarity with other movies.
3. Sorts movies based on similarity.
4. Returns the most similar movies.

---

## 🖥️ Running the Project Locally

### Step 1 — Clone the repository

```bash
git clone https://github.com/YOUR-USERNAME/movie-recommendation-system.git
```

### Step 2 — Navigate to the project

```bash
cd movie-recommendation-system
```

### Step 3 — Install dependencies

```bash
pip install -r requirements.txt
```

### Step 4 — Run the Streamlit application

```bash
python -m streamlit run app.py
```

The application will open in your browser.

---

## 📸 Application

The Streamlit application allows users to select a movie and receive a list of recommended movies based on content similarity.



---

## 🧠 Recommendation Approach

This project uses **Content-Based Filtering**.

Instead of depending on ratings from other users, the system recommends movies based on the characteristics of the selected movie.

For example:

```text
Selected Movie
      ↓
Movie Features
      ↓
Feature Vector
      ↓
Cosine Similarity
      ↓
Similarity Ranking
      ↓
Recommended Movies
```

---

## 📈 Future Improvements

Some possible improvements include:

* 🔥 Add movie posters using the TMDB API
* ⭐ Include ratings and popularity in recommendations
* 👤 Add user-based recommendations
* 🤝 Implement collaborative filtering
* 🧠 Build a hybrid recommendation system
* 🔎 Improve movie search functionality
* ☁️ Deploy the application online
* 📱 Improve the UI/UX
* 🎯 Personalize recommendations based on user preferences

---

## 🎯 Learning Outcomes

Through this project, I learned and practiced:

* Data preprocessing
* Feature engineering
* Natural Language Processing concepts
* Vectorization
* Cosine similarity
* Recommendation systems
* Machine learning workflows
* Streamlit application development
* Git and GitHub project management

---

## 👨‍💻 Author

**Kavya Dinesh Gour**

BTech CSE Student | Aspiring Data Analyst.



