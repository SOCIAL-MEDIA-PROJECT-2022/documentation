# Follower Feature
 
## Description

This feature allows you to subscribe to posts from a User. All posts from followed Users will show up in the User’s post feed.


 
## Authors
- Gordon Ramsbottom
- James Walker
- Hector Rios
- Matt Myers


## Back-End
Inside the Follower Controller file, there is a method called “follow” which passes in three parameters: 1. ID of the current User 2. Email of the followed User 3.  Opposite value of the follow “state”. The follow “state” helps determine if the User is already being followed by the current User. Once the values are passed through the method, a new Follower Object is created and is added to the current User’s follow list, which is a list made of follower objects. In lieu of using User objects consisting of sensitive User information, we utilized Follower Objects, whose values only contain necessary information for a follower list. When visiting a webpage, the backend passes the current User’s follow list to determine the state of the follow button.




## Front-End
The front end of the Follow feature consists of a functional button located within the user card next to the post feed when visiting another User’s page. When the button is initially clicked, the User will be subscribed to all new posts from the followed User. A User who you are following is determined by a follow “state” string containing either the value “follow” or “unfollow” on each User’s page.  When the button is clicked, the string value will change to the other value, including when you hit the button a second time after following a User to effectively “Unfollow” that User. The button text will reflect the opposite of the current follow “state” to allow Users to continue to follow and unfollow a User.

