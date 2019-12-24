# OAuth test project with passportJs.

```diff
- OAUTH a way for users to authenticate using 3rd party apps such as facebook google.
- In this project we will use google+ API to authentication users. 
```

#### This application is to test running an application OAUTH scheme authentication.
#### We will be using passport.js
#### We will be hosting the application in docker container.
#### Source: https://github.com/iamshaunjp/oauth-playlist


### Plan
- We will be talking and retriving info from google. 
- Check image below where yellow shows where we are going to use passport
!()[]


### Usage:
- Make sures
  - npm/node and 
  - Express
  - Docker
  - ejs to render a website. npm install ejs 
- Pull this repo and run following to build the image --> docker build -t nodeexpress .
- Run the container --> docker run -p 3030:8080 -d nodeexpress
- Open in  chrome --> http://localhost:8080
- to stop the application RUN --> docker copntainer THEN docker container stop 9e13d736c9d2


### Routes
- We dont want our code to look messy so we want to modulerize our code. 
```diff
homePage  -> localhost:8080/
loginPage -> localhost:8080/auth/login - Another page that will be visted when click on login.
logoutPage -> localhost:8080/auth/logout -If user wants to logout.
Auth-URL -> localhost:8080/auth/google
```


### Install Passport setup 
- npm install passport passport-google-oauth20
- 
