# 🎬 Movie Recommender System – TMDB Dataset

This is a **beginner-friendly content-based movie recommender system** built using the **TMDB (The Movie Database) dataset**. It uses **cosine similarity** to recommend movies based on content such as genres, keywords, cast, and more.

---

## 🚀 What This Project Does

This system recommends movies that are **similar in content** to a selected movie. It uses:

- 🧠 **Natural Language Processing (NLP)** to process movie data
- 🧮 **Cosine Similarity** to compare movie vectors
- 📊 **Pandas & Scikit-learn** for data processing and modeling

---

## 🧠 How It Works 

1. **Movie Features Combined**: We combine features like **genre, cast, director, overview, etc.** into a single string.

2. **Vectorization**: This combined string is transformed into numerical vectors using `CountVectorizer`.

3. **Cosine Similarity**: We compare all movie vectors using cosine similarity (a math technique that measures how similar two movies are in terms of their content).

4. **Recommendation Output**: For any given movie, we return the **top 5-10 most similar movies**.

---

## ❓ Common Confusions 
1. What is content-based filtering?
It recommends movies based only on their own details — like genre, cast, overview, etc.
It doesn’t depend on other users' ratings or behavior.

2. Why are we using cosine similarity?
It's a math method to measure how similar two movies are based on their content.
The more similar the words (features), the closer they are.

3. What does CountVectorizer do?
It converts text (like genres, overview, keywords) into numbers so that we can compare them using cosine similarity.

4. Why didn’t we use ratings or reviews?
That’s part of collaborative filtering, which is a different type of recommendation system.
This project is focused on content-based filtering only.

5. Will it recommend only same-genre movies?
Not exactly — since we combine multiple features like cast, overview, and keywords, the system can find deeper similarities, not just genre.

---
## ✅ How to Run It
1. Clone the repo:
```bash
git clone https://github.com/your-username/movie-recommender-system-tmdb-dataset.git

Run the Python script:
python app.py