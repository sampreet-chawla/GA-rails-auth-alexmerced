# GA-rails-auth-alexmerced
GA Ruby on Rails authentication using JWT - From Alex Merced Tutorials


The code implementation is a practice session for Ruby on Rails authentication using JWT.
Source, Coding Tutorials Blog - [Ruby on Rails API with JWT Auth Tutorial](https://tuts.alexmercedcoder.com/ruby-tut/)

### Testing Environment

 - Ruby version - ruby 2.7.2p137
 - Rails version - Rails 6.0.3.4
 - Postgres Version - postgres (PostgreSQL) 13.0
 - vscode on Windows 10 - 1.51.0
 - POSTMAN - any latest version would suffice
 
 ### Testing Instructions
 
 - Step 1: Download the code
 - Step 2: bundle install
 - Step 3: Check the /db/seed.rb for admin details
 - Step 4: Start the rails server at port 4000 (rails server -p 4000) - 400 port was used for testing and is used in Postman. Please refer snapshots below and change port as desired.
 - Open Postman, and test the following URLs - 
  *POST localhost:4000/login - Note the token from successful login. It will be required for authentication
  *GET localhost:4000/auto_login - Auto login for an authorized user
  *POST localhost:4000/notes - To create a note for an authorized user
  *GET localhost:4000/notes - To fetch all notes for the authorizes user 


### Testing Snapshots

- Login by an authroized user

  [](./img/01-login.png)
  
- Auto-Login by an authorized user

 [](./img/02-auto-login.png)
 
 - Create note for an authorized user - Notice the Authorization header with bearer and token string
 
  [](./img/03-create-note-for-authorized-user.png)
  
  - Unauthorized access of notes
  
  [](./img/03-unauthorized-access.png)
  
  - Get notes for authorized user
  
    [](./img/04-gett-notes-for-authorized-user.png)



