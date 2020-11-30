# Movie-Recommendation-System on MovieLens
Link to dataset
https://www.kaggle.com/grouplens/movielens-20m-dataset


Instructions to test the recommendation:-
1)Change the call to movie_recommendation()
function by only changing the userId (argument given) with any other userId. This is to test pearson correlation for collaborative recommendation

2)Change the call to movie_recommendation_euclidean() function by only changing the userId (argument given) with any other userId. This is to test Euclidean distance for collaborative recommendation.

3)Path to load the dataset can be changed ,as per your directory

Movie recommendation using Euclidean:-

movie_recommendation_euclidean():-
The only parameter required is the user id. For the given user id, the code gives a recommendation list of movies based on his/her ratings on similar movies.
To calculate the similarity it uses the Euclidean distance formula between the ratings of the common movies and  between the target user and all the other users.


Movie recommendation using Pearson coefficient:-

movie_recommendation():-
The only parameter required for this is userId. It recommends movie by calculating similarity between users by using Pearson correlation formula and then sorts the list obtained, hence giving the movies with the highest similarity.

Other functions:-
pearson_coeff(user1, user2):- needs two parameters that is two user ids, it then calculates similarity by using commonly rated movies between the two users and returns the Pearson coefficient.

euclidean_dist():-needs two parameters that is two user ids, it then calculates similarity by calculating the distance between common rated movies between the two users and returns the distance.

get_movie_title(): takes in a movie Id and returns its corresponding movie title given in the dataset.

get_rating(): takes two params, userid and movieid and returns the corresponding rating given by the user for the movie  in the dataset.

get_movie_title(): takes one parameter, movieId and returns the corresponding movie title given in the dataset.




Content Based:
content_recommendation(title, cosine_sim = cosine_sim):-

Takes input title entered by the user and cosine similarity matrix of movies.
Calculates similar movies to a given movie from the matrix and returns 10 most similar movies .

add_user(userid,movies,usr_rating):
userid -The userid of the new user to be added to the database
movies-List containing the movie ids watched by the new user
rating -List containing rating ratings of the respective movies watched by the user in movies list

