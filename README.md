MOVIE RECOMMENDATION SYSTEM

-Project Overview
This project builds a Movie Recommendation System using Python and machine learning techniques. The system recommends movies to users based on similarity between movie features such as overview, genres, keywords, cast, and crew.
The recommendation engine uses TF-IDF vectorization and cosine similarity to measure how similar movies are to each other and generate personalized recommendations.

-Objective
The main goal of this project is to develop a content-based recommendation system that suggests movies similar to a given movie title.

-Dataset
dataset link: https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata
The project uses the TMDB 5000 Movie Dataset, which contains information about thousands of movies including:
•	Movie title
•	Overview (description)
•	Genres
•	Keywords
•	Cast
•	Crew
•	Popularity and ratings
Dataset files used:
•	tmdb_5000_movies.csv
•	tmdb_5000_credits.csv
These datasets are merged to create a single dataset for analysis.

-Technologies Used
•	Python
•	NumPy – Numerical computations
•	Pandas – Data manipulation and preprocessing
•	Scikit-learn – Machine learning utilities
•	TF-IDF Vectorizer – Converts text data into numerical vectors
•	Cosine Similarity – Measures similarity between movies

-How the Recommendation System Works
1. Data Loading
The movie and credits datasets are loaded using Pandas.
2. Data Merging
The datasets are merged based on the movie title to combine movie details with cast and crew information.
3. Feature Selection
Important movie features are selected:
•	Title
•	Overview
•	Genres
•	Keywords
•	Cast
•	Crew
These features help describe each movie.
4. Feature Combination
The selected features are combined into a single text column called combined_features.
5. Text Vectorization
The TF-IDF Vectorizer converts the combined movie text into numerical vectors.
6. Similarity Calculation
Cosine similarity is used to calculate how similar each movie is to every other movie.
7. Recommendation Generation
When a movie title is entered, the system:
1.	Finds the movie in the dataset
2.	Computes similarity scores
3.	Returns the top most similar movies

-Example Usage
print(get_recommendations("Harry Potter and the Half-Blood Prince"))
Output: A list of recommended movies similar to the selected movie.


-How to Run the Project
1. Install Required Libraries
pip install numpy pandas scikit-learn
2. Open the Notebook
Run the notebook using Jupyter Notebook or Google Colab.
3. Run All Cells
Execute the notebook cells to build the recommendation system and generate movie suggestions.


-Conclusion
This project demonstrates how content-based recommendation systems can be built using machine learning techniques. By analyzing movie features and calculating similarity scores, the system provides relevant movie suggestions to users.

