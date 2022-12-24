# Tinder Clone (movieConnect) - ReactJs, NodeJs, MySQL, WebSockets, JWT


## Description:

This project was made as a way to practice using Web Sockets.
This project replicats the famous swipe animation that Tinder uses, and it exemplifies
several small features present in most dating apps. I made a
WebSocket API for my backend using a Socket.io server, which allowed
two-way communication between client apps and the backend. 
First the API lets users register with a username, password, and profile. Then
saves the credentials in a JawsDB MySQL database. The API handles user actions such as
like/disliking movies, accepting matches, chatting with matches, and profile editting is saved to 
the database.
<br>
<br>
<a href="https://movieconnect.netlify.app/" target="_blank" >Live Demo</a>
> Preview
<p>
<img src="https://github.com/ChrisCash2020/Images/blob/master/movie/demo.gif" />
</p>

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
- JSON Web Token

## Top Features:
- Bcrypt password encryption/verification
- Multer file upload of profile images
- JWT authentication and authorization
- Filtered matching system based on preferences and movie interests
- Genre based movie recommendation filtering as well as favorited movie filtering
- Movie recommendation refreshing 
- Bcrypt password encryption/verification

## Design:

### Client-side:

This is the front-end repository

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
The back-end repository: <a href="https://github.com/ChrisCash2020/movie-connect-server/" target="_blank" >movieConnect</a>

Socket.io Server: 
- Express server:
  - Module-View-Controller project structure
  - Manually contructed User model NO-ORM
  - Store User profile images in static folder on server
  - User Authenication done through secure HTTP only JWT

### Database:

Tables:
- Users: stores username, password, status, bio, name, gender, preference, image, and birthday
- Favorites: stores title id as movie favorite, the username id, and the type of favorite
- Chats: stores text, username id, author (name field in Users), roomId, and time chat sent
- Rooms: stores roomId, username 1 (sender), username 2 (recepient)



  
