# Tinder Clone (movieConnect) - ReactJs, NodeJs, MySQL, WebSockets


## Description:

This project was made as a way to practice my WebSockets development.
It replicats the famous swipe animation that Tinder uses, and it exemplifies
several small features present in the real website. I made a
WebSocket API for my backend using Socket.io Server, which allowed a
two-way communication between client apps and your backend. 
The user can create a username, password, and profile, which all get
saved in a JawsDB MySQL database. All user actions from like/dislike 
movies, accepting matches, chatting with matches, editing profile is collected to 
the database.
<br>
<br>
<a href="https://chriscash2020.github.io/movie-client/" target="_blank" >Live Demo</a>

## Installation

<pre>
cd movie-client
npm install 
npm run dev
</pre>

## Technologies Used:

- ReactJS
- NodeJS
- ExpressJS
- Socket.io
- MySQL
- TmdbAPI

## Design:

### Client-side:

This is the front-end repository

> Preview
<p>
<img src="https://github.com/ChrisCash2020/Images/blob/master/movie/demo.gif" />
</p>

<br/>

> Routes
<p float="left">
<img src="https://github.com/ChrisCash2020/Images/blob/master/movie/home.png" width="180" height="360" />
<img src="https://github.com/ChrisCash2020/Images/blob/master/movie/match.png" width="180" height="360" />
<img src="https://github.com/ChrisCash2020/Images/blob/master/movie/msg.png" width="180" height="360" />
<img src="https://github.com/ChrisCash2020/Images/blob/master/movie/prof.png" width="180" height="360" />
</p>

<br/>

> Error Handling
<p float="left">
<img src="https://github.com/ChrisCash2020/Images/blob/master/movie/login.png" width="180" height="360" />
<img src="https://github.com/ChrisCash2020/Images/blob/master/movie/name.png" width="180" height="360" />
<img src="https://github.com/ChrisCash2020/Images/blob/master/movie/img.png" width="180" height="360" />
<img src="https://github.com/ChrisCash2020/Images/blob/master/movie/bday.png" width="180" height="360" />
<img src="https://github.com/ChrisCash2020/Images/blob/master/movie/bday2.png" width="180" height="360" />
<img src="https://github.com/ChrisCash2020/Images/blob/master/movie/gen.png" width="180" height="360" />
<img src="https://github.com/ChrisCash2020/Images/blob/master/movie/pref.png" width="180" height="360" />  
</p>


### Server-Side:
The back-end repository: <a href="https://github.com/ChrisCash2020/movie-connect-server1/" target="_blank" >movieConnect</a>

Socket.io Server: 
- Express server:
  - Module-View-Controller design pattern
  - Manually contructed a User model, controller, and routing
  - In-house SQL queries used to facillitate database requests
  - Store User profile images in static folder on server

### Database:

Tables:
- Users: stores username, password, status, bio, name, gender, preference, image, and birthday
- Favorites: stores title id as movie favorite, the username id, and the type of favorite
- Chats: stores text, username id, author (name field in Users), roomId, and time chat sent
- Rooms: stores roomId, username 1 (sender), username 2 (recepient)



  
