# KNN-Recommendation-Engine

This project is a simple book recommendation system implemented in Python. It uses a K-Nearest Neighbors (KNN) model to recommend books that are similar to a given book. The recommendations are based on user ratings.

## Code Overview
The code first loads a dataset of books and ratings. It then preprocesses the data by removing missing values and filtering out users who have rated fewer than 200 books and books that have been rated by fewer than 100 users.

The preprocessed data is then transformed into a user-item matrix, where the rows represent books, the columns represent users, and the cells contain ratings. If a user hasn't rated a book, that cell is filled with 0.

A KNN model is then trained on this matrix using cosine similarity as the distance metric.

The get_recommends function takes a book title as input and returns a list of 5 books that are most similar to the input book, based on the KNN model. The similarity is determined by the user ratings of the books.
