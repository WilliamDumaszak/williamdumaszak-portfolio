Movie Recommendation System Using Cosine Similarity and NLP

Welcome!
In this project, we apply cosine similarity to build a movie recommendation system based on the similarity of movie characteristics. In addition, we use Natural Language Processing (NLP) techniques to preprocess textual data.

The dataset used is the TMDB 5000 Movie Dataset, which contains metadata for over 5,000 movies. It is publicly available on Kaggle via the following link:
👉 TMDB 5000 Movie Metadata on Kaggle

⸻

📊 Project Steps

1. Data Exploration and Preprocessing
We start by exploring and cleaning the dataset. In this step, we use Python’s ast module (Abstract Syntax Trees) to safely convert stringified Python-like dictionaries into usable Python objects.

2. Data Cleaning and Feature Engineering
We remove blank spaces and create a new feature called tags, which combines relevant information from different columns into a single text string. This will be used as the input for our vectorizer.

3. Text Normalization with Stemming
Before applying the vectorizer, we use stemming (via PorterStemmer) to reduce words to their root forms. This ensures that similar words like “run”, “running”, and “ran” are treated as the same term.

4. Vectorization
Using CountVectorizer, we transform the tags into numerical vectors, where each column represents a word and each row represents a movie, with values indicating word frequencies.

5. Recommendation Engine
Finally, we compute cosine similarity between movie vectors to identify the top 5 most similar movies based on any selected movie. The system returns recommendations using content-based filtering.

⸻

To get started with the project, clone the repository, install the required dependencies using requirements.txt, and run the Jupyter Notebook cell by cell.