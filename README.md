# BookBuffet - Book Recommendation System

**BookBuffet** is a sophisticated book recommendation system developed using the **Flask** framework. This system leverages various datasets, including books, ratings, and user information, to provide personalized book recommendations to users. Whether you're a book enthusiast or looking to find your next read, BookBuffet uses collaborative filtering and content-based algorithms to suggest books based on your preferences.

## Business Problem

In the age of information overload, selecting the right book can be overwhelming. Traditional book recommendation methods often fail to provide personalized suggestions based on individual preferences. The goal of this project is to build a recommendation system that provides book recommendations based on user ratings, book features, and user behavior. 

## Key Features

- **Personalized Recommendations**: Get book suggestions based on your previous ratings and preferences.  
- **Collaborative Filtering**: Recommender based on the ratings of users who have similar tastes.  
- **Content-Based Filtering**: Suggestions based on the attributes of books (e.g., genre, author).  
- **Search Functionality**: Users can search for books by title or author and get personalized recommendations.  
- **Flask-based Web Application**: A user-friendly interface that allows users to interact with the recommendation system.

## Data

The system is built using the following datasets:

- **Books Dataset**: Contains information about books such as title, author, genre, etc.  
- **Ratings Dataset**: Contains ratings given by users to various books.  
- **Users Dataset**: Contains user details that allow us to personalize recommendations based on individual preferences.

### Source

The datasets used in this project are publicly available and were obtained from the following sources:

- [Books Dataset](https://www.kaggle.com/datasets)
- [Ratings Dataset](https://www.kaggle.com/datasets)
- [Users Dataset](https://www.kaggle.com/datasets)

## Analysis Approach

The recommendation system uses two primary techniques to suggest books:

1. **Collaborative Filtering**: This technique finds similar users and recommends books that users with similar tastes have enjoyed.  
2. **Content-Based Filtering**: This technique recommends books based on the attributes of the books, such as genre, author, and description.

### Algorithms

- **Cosine Similarity**: Used for calculating the similarity between books or users.  
- **Matrix Factorization**: Decomposes user-item interaction matrices to predict ratings for unseen books.

## Tools and Technologies Used

- **Flask**: A lightweight web framework for building the web application.  
- **Python**: Programming language for data analysis and machine learning model development.  
- **Pandas & NumPy**: For data manipulation and analysis.  
- **Scikit-Learn**: For machine learning algorithms and model building.  
- **Cosine Similarity**: For comparing user-item similarity.  
- **Pickle**: For saving trained models and similarity scores.  
- **HTML, CSS**: For the frontend of the web application.

## Project Structure

```plaintext
bookbuffet/
│
├── app.py                         # Flask application to serve the recommendation system
├── EDA_on_dataset.ipynb           # Exploratory Data Analysis on the datasets
├── requirements.txt               # Python dependencies for the project
├── Books.csv                      # Dataset containing book information
├── Ratings.csv                    # Dataset containing user ratings for books
├── Users.csv                      # Dataset containing user information
├── books.pkl                      # Pickled model for book data
├── similarity_scores.pkl          # Pickled model for similarity scores
├── popular.pkl                    # Pickled model for popular books
└── README.md                      # Project documentation
```

How to Run the Application
Clone the repository:
git clone https://github.com/your-repo/bookbuffet.git

cd bookbuffet
Install dependencies:
Ensure you have Python 3.x installed, then run:
pip install -r requirements.txt

Run the Flask Application:
Start the Flask app by running the following command:
python app.py

Access the application:
Open your browser and go to http://127.0.0.1:5000/ to use the book recommendation system.
