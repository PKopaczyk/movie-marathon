# movie-marathon

The goal of this program is to create structure for movies enthusiasts to pick their favourit movies for marathon. All users can enter their prefered movies which they want to watch, or they can delete the movie from their list.  
Users and movies are identified by their unique number. All users create a tree where every user can add new users as children to his node. At the beginning there is a root with undetified by number 0. Every node except for root can be deleted from the tree.  
Movies are identified by users by their number which is at the same time the rating given by the user for specific movie (so two different movies cant be rated the same by one user).

Program provides following operations:

addUser [parentUserId] [userId]  

delUser [userId]  

addMovie [userId] [movieRating]  

delMovie [userId] [movieRating]  

marathon [userId] [k] - displays at most k movies wich are all rated highest by user userID OR movies generated by applying marathon function to all descendants of userID and additionally picking from them all movies rated higher then the highest rating from all movies added by userID
