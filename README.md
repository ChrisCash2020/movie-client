# Tinder Clone - ReactJS, NodeJS, Mysql, WebSockets


## Description:

This project was made in as a way to practice my WebSockets skills.
I also used it to practice my back-end RestAPI development. It replicats the
famous swipe animation that Tinder uses, and it exemplifies
several small features present in the real website. I made a
WebSocket API for my backend using Socket.io Server, which allowed a
two-way communication between client apps and your backend. 
The user can create a username, password, and profile, which all get
saved in a JawsDB MySQL database. All user actions from like/dislike 
movies, accepting matches, chatting with matches, editing profile is collected to 
the database.

## Time Taken:

2.5 weeks

## Technologies Used:

- ReactJS
- NodeJS
- ExpressJS
- Socket.io
- MySQL
- TmdbAPI

### Front End:


The front-end is hosted on GitHub. 
This repository is the front-end

### Back End

The back-end repository is: https://github.com/ChrisCash2020/movie-connect-server1/


## Design:

### Database:

4 Tables:
- Users: Stores username, password, status, bio, name, gender, preference, image, and birthday
- Favorites: Stores title id as movie favorite, the username id, and the type of favorite
- Chats: Stores text, username id, author (name field in Users), roomId, and time chat sent
- Rooms: Stores roomId, username 1 (sender), username 2 (recepient)


### Server-Side:
Socket.io Server: 
- Express server:
  - Mutations and queries are sent to the front end.
  - Constructed a User model to facilliate database requests
  
### Front-End:

Front End fully developed in ReactJS using Vite
