# Nates-MVC: Tech Blog
Model View Controller using MYSQL/Express

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## Description.

Nates' MVC Tech Blog is a Heroku deployed application, which serves as a CMS-style platform designed for the technologically inclined. It allows those in the tech communtiy to publish blog posts based on their experiences within the Tech industry. Additionally there is a comment section that allows users to interact and engage with another on Blog posts. The application uses MVC with Handlebars.js as the template, Sequelize as the ORM, and the express-session npm package handles authentication. This App used 

## Table of Contents:
- [Overview](#Overview)
- [The Challenge](#The-Challenge)
- [Usage Information](#Usage-Information)
- [Installation Process](#Installation-Process)
- [Built With](#Built-With)
- [What I Learned](#What-I-Learned)
- [Future Development](#Future-Development)
- [License](#License)
- [Author](#Author)
- [Acknowledgments](#Acknowledgments)

# Overview

## The Challenge:

The challenge of building this application involved creating a scalable and robust platform that could support multiple users, blog post and comments. The application was designed with security in mind, allowing users to authenticate themselves and protect their personal data. Furthermore, the application had to be built using modern web development technologies and follow best practices, including the MVC architecture pattern.

## Assigned User Story:
```
AS A developer who writes about tech
I WANT a CMS-style blog site
SO THAT I can publish articles, blog posts, and my thoughts and opinions
```
## Acceptance Criteria:
```
GIVEN a CMS-style blog site
WHEN I visit the site for the first time
THEN I am presented with the homepage, which includes existing blog posts if any have been posted; navigation links for the homepage and the dashboard; and the option to log in
WHEN I click on the homepage option
THEN I am taken to the homepage
WHEN I click on any other links in the navigation
THEN I am prompted to either sign up or sign in
WHEN I choose to sign up
THEN I am prompted to create a username and password
WHEN I click on the sign-up button
THEN my user credentials are saved and I am logged into the site
WHEN I revisit the site at a later time and choose to sign in
THEN I am prompted to enter my username and password
WHEN I am signed in to the site
THEN I see navigation links for the homepage, the dashboard, and the option to log out
WHEN I click on the homepage option in the navigation
THEN I am taken to the homepage and presented with existing blog posts that include the post title and the date created
WHEN I click on an existing blog post
THEN I am presented with the post title, contents, post creator’s username, and date created for that post and have the option to leave a comment
WHEN I enter a comment and click on the submit button while signed in
THEN the comment is saved and the post is updated to display the comment, the comment creator’s username, and the date created
WHEN I click on the dashboard option in the navigation
THEN I am taken to the dashboard and presented with any blog posts I have already created and the option to add a new blog post
WHEN I click on the button to add a new blog post
THEN I am prompted to enter both a title and contents for my blog post
WHEN I click on the button to create a new blog post
THEN the title and contents of my post are saved and I am taken back to an updated dashboard with my new blog post
WHEN I click on one of my existing posts in the dashboard
THEN I am able to delete or update my post and taken back to an updated dashboard
WHEN I click on the logout option in the navigation
THEN I am signed out of the site
WHEN I am idle on the site for more than a set time
THEN I am able to view comments but I am prompted to log in again before I can add, update, or delete comments
```

## GIF:
### Tech Blog GIF

The following animation demonstrates the application functionality:
![](/GIF01.gif)

## Usage Instructions:

#### Visit the homepage, "Login" or "Sign Up" for an account if you don't already have one.

1. Option: A) Account login: click on "login" in the navigation menu - enter Username and Password then click "Sign In" to proceed.
1. Option: B) Account Sign Up: click on "Sign Up" in the navigation menu - once open, enter Username, Email and Password then click "Sign Up" to proceed.
2. Once you have an account, you can create blog posts and comment on other users' posts.
3. Create a blog post: click on the "dashboard" option in the navigation menu and select "Create a New Blog Post."
4. Enter a title and contents for your Blog Contribution, then click "Create Post" to save and publish.
5. View existing blog posts by clicking on "Home" in the navigation menu.
6. Comment: to view or "add a new comment" go to any blog post, click on any blog post - once open, you may view the comment history as well as add a new comments.
7. Edit or delete your blog post: click on the "dashboard" option in the navigation menu and select the post you wish to edit or delete.
8. Account Log out: click on "logout" in the navigation menu.

## Deployed Application Link:
[Deployed Application on Heroku Link:](https://infinite-harbor-72074-59c627de35a2.herokuapp.com))

## YouTube Walkthrough Video:
[Click Here to Watch](https://youtu.be/7hvVSYC_0NA)

## Screenshot:
![](/SS01.png) 

## Installation Process
1. Clone the Repository from GitHub 
(or) Download Zip Folder from Repository from GitHub
Open the cloned (or downloaded) repository in any source code editor.
2. Open the repository and run:
```console 
npm init -y
```
3. make a .env file in the root directory with your corresponding MySQL DB_NAME, DB_USERNAME, DB_PASSWORD
4. Run the MYSQL command line:
```console
mysql -u root -p
source db/schema.sql
use tech_blog_db
\q
```
4. Now to seed and start the server:
```console
npm i
npm run seed
npm start
```
5. Naviagte towards: [http://127.0.0.1/3001](http://127.0.0.1/3001) to test the app!

## Built With:
- JSON:[ JSON](https://www.npmjs.com/package/json)
- Dynamic JavaScript
- Node.js [Version 16.18.1](https://nodejs.org/en/blog/release/v16.18.1/)
- Express.js:[Express.js](https://expressjs.com/en/starter/installing.html)
- Bcryptjs: [5.0.1](https://www.npmjs.com/package/bcryptjs)
- Connect Session Store using Sequelize: [7.1.1](https://www.npmjs.com/package/connect-session-sequelize)
- Dotenv: [9.0.2](https://www.npmjs.com/package/dotenv)
- Express: [4.17.1](https://www.npmjs.com/package/express)
- Express Handlebars: [5.3.2](https://www.npmjs.com/package/express-handlebars)
- Express-Session: [1.17.1](https://www.npmjs.com/package/express-session)
- Handlebars.js: [5.3.2](https://www.npmjs.com/package/handlebars)
- Node MySql2: [2.2.5](https://www.npmjs.com/package/mysql2)
- Sequelize: [6.6.2](https://www.npmjs.com/package/sequelize)
- License Badge: [Shields.io](https://shields.io/)
- Visual Studio Code: [Website](https://code.visualstudio.com/)

## What I Learned:
1. Implementing the Model-View-Controller (MVC) architecture and understanding how the MVC works.
2. Creating and interacting with a MySQL database using Sequelize with Object Relational Mapping.
3. Creating and using Express.js servers & routes.
4. Using Handlebars.js to create and display dynamic templates.
5. Implementing bcrypt for user authentication.
6. Using Bootstrap for the styling and layout.

### Future Development:
1. Add a Dark/Light mode feature?
2. Pagination for blog posts and comments.
3. The ability to edit and delete comments.
4. Add User Profile pages.

## License & Copyright ©
  
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [Open Source Initiative Link](https://opensource.org/licenses/MIT)

### Copyright © 2023 Nathan Weekley
```md
Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

## Author

© 2023 [Nathan Weekley](https://github.com/Nweekley84). Confidential and Proprietary. All Rights Reserved.
