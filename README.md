# Tinder Clone (movieConnect) - ReactJS, NodeJS, Mysql, WebSockets


## Description:

This project was made as a way to practice my WebSockets development.
I also used it to practice my back-end RestAPI development. It replicats the
famous swipe animation that Tinder uses, and it exemplifies
several small features present in the real website. I made a
WebSocket API for my backend using Socket.io Server, which allowed a
two-way communication between client apps and your backend. 
The user can create a username, password, and profile, which all get
saved in a JawsDB MySQL database. All user actions from like/dislike 
movies, accepting matches, chatting with matches, editing profile is collected to 
the database.
<br>
<br>
<a target="_blank" href="https://chriscash2020.github.io/movie-client/">Live Demo</a>

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

The back-end repository: <a target"_blank" href="https://github.com/ChrisCash2020/movie-connect-server1/">movieConnect</a>


## Design:

### Front-End:

Front End fully developed in ReactJS using Vite

### Server-Side:
Socket.io Server: 
- Express server:
  - Module-View-Controller design pattern
  - Manually contructed a User model, controller, and routing
  - In-house SQL queries used to facillitate database requests

### Database:

Tables:
- Users: stores username, password, status, bio, name, gender, preference, image, and birthday
- Favorites: stores title id as movie favorite, the username id, and the type of favorite
- Chats: stores text, username id, author (name field in Users), roomId, and time chat sent
- Rooms: stores roomId, username 1 (sender), username 2 (recepient)



  
