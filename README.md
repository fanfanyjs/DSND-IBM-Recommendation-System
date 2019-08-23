# DSND-IBM-Recommendation-System

## Description
This project is one of Udacity's Data Science Nanodegree assignments. It utilises data from IBM Watson Studio Platform to build three types of article recommendation system for its users:

- Rank based recommendation: Recommending most popular articles
- User-user based recommendation: Recommending articles that similar users have viewed
- Content based recommendation: Recommending articles that are similar to what the user has read

## Methodology

#### Rank-based
This is carried out purely by sorting the articles based on number of unique views. This recommendation system is more suitable for new users without any history indicating their interests.

#### User-user based
For each user, a list of similar users are chosen based on dot product. The user is then recommended items that similar users have read.

#### Content-based
NLTK techniques are used to preprocess titles (e.g. tokenize, normalise, lemmatize) of the articles read by each user. Then, similar articles are identified based on dot product and are recommended to users.

#### Matrix Factorization
Last but not least, I also optimised the number of latent features using Singular Vector Decomposition to predict the articles that will be subsequently read by each user.


## Dependencies
Python 3.5 is used to create this project and the following libraries are used:

- Machine Learning Libraries: NumPy, Pandas, Sciki-Learn
- Natural Language Processing: NLTK
- Regex: re
- Serialising Python Object Structure: Pickle


## Credits
Udacity and IBM - for providing the dataset and designing the project
