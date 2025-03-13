# To-Do Application API

This is a RESTful API for a To-Do application, built using Node.js, Express, and MongoDB. The application supports user authentication using jsonwebtoken and  supports crud operation for both users and tasks.

## Features
- User authentication using json web token(Register/Login)
- Create, Read, Update, and Delete  operations for tasks
- Secure API endpoints using JWT authentication
  
##Setup
1.Inialize the nodejs server using npm init command
2.Install necessary libararies like nodemon,express,mongoose,dotenv,bcrypt,jsonwebtoken using npm i
3.Store the Port no,mongourl and jwt secret key in .env file
4.Add the files that are not needed to push to the git in the .gitignore file
5.Setup the database and create models for both the Task and User
6.create routes in the routes folder for authentication,user routes and tasks routes
7.Create a authenticate middleware in for authentication purpose
8.Test the APIs in the thunder client.

