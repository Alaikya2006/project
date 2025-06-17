# 🎬 Movie Recommendation System (Content-Based Filtering)

This project builds a **Movie Recommendation System** using content-based filtering based on movie genres. The system recommends movies that are similar in genre to a movie selected by the user.

---

## 💡 **Objective**
- Recommend similar movies based on genre information.
- Help users discover new movies similar to their preferences.

---

## 📂 **Dataset**
- **Source:** [The Movies Dataset - Kaggle](https://www.kaggle.com/datasets/rounakbanik/the-movies-dataset)
- **File used:** `movies_metadata.csv`
- Contains metadata about ~45,000 movies including genres.

---

## ⚙ **Technologies & Libraries**
- Python
- Pandas
- scikit-learn
- Jupyter Notebook

---

How it works
1. Data Preprocessing
   - Load and clean the dataset.
   - Parse genres from JSON format to plain text.
   - Remove duplicates and empty genres.
   - For memory efficiency, work with a subset (e.g., first 1000 movies).

2. Vectorization
   - Use `CountVectorizer` to convert genre text into numerical feature vectors.

3. Similarity Computation
   - Compute cosine similarity between movie vectors.

4. Recommendation
   - Given a movie title, find the top 5 most similar movies.

---

Example
`python
recommend_movie("Toy Story", df, similarity)

How to run
1️ Clone/download this repository.
2️ Download movies_metadata.csv from Kaggle and place it in your project directory.
3️ Run the Jupyter Notebook.
4️ Install dependencies if needed:

bash
Copy
Edit
pip install pandas scikit-learn
