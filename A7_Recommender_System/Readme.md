# **Movie Recommender** 
**---------------------------------------**

## **Workflow**
*--------------*

### - what i did was simply i took the first 200 User and check what movies they have seen from the first 200 movies 
### - dropped the useless columns
### - then i created pivot_table from the data left
### - created a movie-movie similarity matrix from the data 
### - created a DataFrame from the movie-movie similarity matrix


## - created a function **recommend_movies_similar_to_movie** where it uses the movie-movie DataFrame to reccomed the similar movies to a given movie


### - created a User-User similarty matrix from the data
### - created a User-User similarity matrix from the data 
### - created a DataFrame from the User-User similarity matrix

## - created a function **recommend_movies_for_user** where it uses the User-User DataFrame to reccomed movies to a given User

********************************************************************************

## **Functions**
*---------------------*

## **recommend_movies_similar_to_movie** : 
-----------------------------------------
### the Arguments are **movie**, **recomemnds**
### **movie** refers to the movie name
### **recomemnds** refers to the number of recomendations 
#### **recomemnds** set to default = 10 

### the function catches the name of the movie and number of recommendations
### in data_matrix[dataframe] movie titles were set to be the indices
### saving the indices means savng the mavie titles
### looping over the indices and printing the recommended movies
### returns the recommended movies

***********************



## **recommend_movies_for_user** : 
-----------------------------------------
### the Arguments are **userID**, **recommends**, **similar_users**
### **movie** refers to the movie name
### **recomemnds** refers to the number of recomendations 
#### **recomemnds** set to be default = 3 
### **similar_users** refer to the number of similar users to get recommeded movies from 
#### **similar_users** set to be deafult = 5

### catching function args
### save the ids of similar users
### loop on those similar users
### saves all the movies that this user watched with high ratings
### check if the user have watched it or not (if user rated that movie or not)
### if the User hasn't watched it recommend the movie
### returns the recommended movies


