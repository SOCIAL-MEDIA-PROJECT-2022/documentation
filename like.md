# Like Post Feature

## Description

This is a feature of the Social Media Project that allows users to like and unlike posts and comments.

## Authors
- EdwinS27
- PatrickShawnNelson

## BackEnd
The Post Controller takes in a LikeRequest object. The object is sent to the Post Service. The post service takes the LikeRequest object's userID and postID and searches for the respective post and user in the database. If both have been found, it will append both values into a joined table between Post and Users called, "Likes." If it has already been confirmed that the user has already liked the post, then it will remove those values from the table, this process would be considered an "un-like."  

## FrontEnd
Established the LikeComponent and Likeservice. LikeService sends a patch request to the backend. LikeComponent grabs relevant user information and post information and sends it to the backend through a patch request via services. Additionally, the LikeComponent will display the length of the array or the number of likes for each post based on information received from the database.