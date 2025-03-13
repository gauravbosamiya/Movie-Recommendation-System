## Movie Recommendation System

Overview
- This project implements a Content-Based Movie Recommendation System using the TMDB 5000 dataset.
- It suggests movies based on movie similarity calculated using textual features like genres, cast, crew, and keywords.

Technologies and Libraries Used:
- Python
- Pandas (for data manipulation)
- NumPy (for numerical computations)
- ast (to convert stringified lists to Python lists)
- Scikit-learn (TfidfVectorizer, Cosine Similarity) (for recommendation system)
- matplotlib , seaborn (for data visulization)

1. Data Preprocessing:

- Dropped missing values.
- Extracted important fields like genres, keywords, cast, and crew.
- Converted them into a proper format.

  
2. Feature Engineering:

- Selected the top 3 cast members.
- Extracted only the director from the crew.
- Created a tag column by merging relevant features.
  
3. Text Processing:

- Used TF-IDF Vectorizer to convert movie tags into numerical vectors.
- Removed stopwords for better recommendations.
  
4. Similarity Computation:

- Used Cosine Similarity to measure movie similarity.
- Computed pairwise similarities to recommend movies.

5. Recommendation System:
- Defined a function to fetch similar movies based on cosine similarity scores.
