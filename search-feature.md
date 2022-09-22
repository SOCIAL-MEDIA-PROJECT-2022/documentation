# Search User Feature

## Description

This feature allows you to search for registered users of the web application.


## Authors
- Mat Mayers
- Hector Rios
- Gordon Ramsbottom
- James Walker


## Back-End
The Search Controller has a getmapping method called “search” which passes in the user input string as a parameter. The database returns a result set which is a list of all registered users’ emails which contain the input string characters within the email name.

## Front-End
Our frontend consists of a search bar , search feed page and post feed page components along with search and search bar services to achieve the search functionality of our front end. These components and services work in concert to provide the logic and services to achieve search functionality. When the profile page is visited inside of the nav bar there is a search bar where you are able to search for registered user by email once the search icon is clicked the search bar service component utilizes the search bar service to make an api call to the back end and the user is routed to the search feed page this is where the search feed page component utilizes the search service to display the profile picture, first name, last name and email of any registered user whose email contains the string that was specified in the search bar.
