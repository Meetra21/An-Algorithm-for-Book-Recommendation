# Books Recommender System using Clustering & Collaborative Filtering  

This project builds a **Books Recommendation System** that suggests books to users based on their interests and preferences.  

The system leverages **Collaborative Filtering** (using user ratings) and **Clustering techniques** to group similar users/books, allowing personalized recommendations. By analyzing how users rate different books, the model can recommend new books that align with a user’s reading habits.  

---

## 🎯 Project Objective  

- Build a system that recommends books to users based on:  
  - **Collaborative Filtering** (users/items similarity from ratings)  
  - **Clustering** (grouping similar users/books)  
- Help readers discover **new books that match their preferences**.  
- Demonstrate a practical use of **machine learning in recommender systems**.  

---

## 📂 Dataset  

- **Source**: [Kaggle – Book Recommendation Dataset](https://www.kaggle.com/ra4u12/bookrecommendation)  
- **Files**:  

1. **BX-Books.csv**  
   - 271,000+ book entries  
   - Fields: ISBN, title, author, publication year, publisher, cover image URL  

2. **BX-Users.csv**  
   - User profiles (ID, location, age)  
   - Helps analyze demographics of book ratings  

3. **BX-Book-Ratings.csv**  
   - Over **1 million ratings** by users  
   - Fields: User ID, ISBN, rating (explicit or implicit)  

---

## 🧭 Workflow  

### 1. Data Preprocessing  
- Load and merge datasets (books, users, ratings)  
- Handle missing values and duplicates  
- Normalize ratings for consistency  

### 2. Exploratory Data Analysis (EDA)  
- Distribution of ratings (explicit vs implicit)  
- Most-rated and highest-rated books  
- Active users and popular authors  

### 3. Modeling  

- **Collaborative Filtering**  
  - User-based similarity: Recommend books liked by similar users  
  - Item-based similarity: Recommend books similar to ones a user has rated highly  

- **Clustering**  
  - Apply clustering algorithms (e.g., KMeans) to group users/books  
  - Use clusters to generate recommendations within similar groups  

### 4. Recommendation Engine  
- Given a user/book → return top N recommended books  

---

## 📂 Repository Structure  

- `data/` – Kaggle dataset files (`BX-Books.csv`, `BX-Users.csv`, `BX-Book-Ratings.csv`)  
- `notebooks/` – Jupyter notebooks for preprocessing, EDA, and model training  
- `models/` – Scripts for clustering & collaborative filtering models  
- `results/` – Recommendation outputs and evaluation reports  

---

## 🚀 How to Run  

1. Clone the repository:  
   ```bash
   git clone https://github.com/your-username/books-recommender-system.git
   cd books-recommender-system
