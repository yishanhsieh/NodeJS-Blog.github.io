# NodeJs, Express, EJS & MongoDB Blog - CRUD

This repo is used for learning to building a NodeJs blog and how to run it on a free host. I am really appreciate Raddy's efforts for the 10 videos and open source code. 


## Video playlists:
1. [Part1](https://www.youtube.com/watch?v=-foo92lFIto&list=PL4cUxeGkcC9hAJ-ARcYq_z6lDZV7kT1xD) : Import npm and all the other required libraries. Build up a HelloWorld page.
2. [Part2](https://www.youtube.com/watch?v=gv3FFnOdCIo&list=PL4cUxeGkcC9hAJ-ARcYq_z6lDZV7kT1xD&index=2): render basic personal information through main.ejs, which renders index.ejs and about.ejs.
3. [Part3](https://www.youtube.com/watch?v=MruZEGPibC4&list=PL4cUxeGkcC9hAJ-ARcYq_z6lDZV7kT1xD&index=3): Layout design on style.css
4. [Part4](https://www.youtube.com/watch?v=FjuctFNN0FA&list=PL4cUxeGkcC9hAJ-ARcYq_z6lDZV7kT1xD&index=4): build up search.ejs, connect to MongoDB, create database schema.
   ** Remember to put on /blog in the end of your MONGODB_URL, or your mongoDB table will be named 'test' automatically, but it still works.
   
6. [Part5](https://www.youtube.com/watch?v=Cz-2QzkuCHo): insert Post data in MongoDB to index.ejs.
   ** DB table is automatically built up after we create schema (in model folder).
7. [Part6](https://www.youtube.com/watch?v=9Bnpl6bcev4&list=PL4cUxeGkcC9hAJ-ARcYq_z6lDZV7kT1xD&index=6): create slug for each blog. create the logics for searchbar.
8. [Part7](https://www.youtube.com/watch?v=FmqBk2UTHzE&list=PL4cUxeGkcC9hAJ-ARcYq_z6lDZV7kT1xD&index=7): create Sign in and register pages in /admin
9. [Part8](https://www.youtube.com/watch?v=uCQirwe5UVg&list=PL4cUxeGkcC9hAJ-ARcYq_z6lDZV7kT1xD&index=8): create cookie, bcrypt(store pwd),  jwt, 
  ** in 8'17 of Part8 video, register page is commented out after registering one admin user, which is saved in the MongoDB USER table.
  ** This episode is not easy. Remember to create JWT in .env. You can check your token from 'inspect'.
10. [Part9](https://www.youtube.com/watch?v=xQVM33SAjLM&list=PL4cUxeGkcC9hAJ-ARcYq_z6lDZV7kT1xD&index=9): create admin dashboard page, add post.
11. [Part10](https://www.youtube.com/watch?v=gR1Zlu4u58g&list=PL4cUxeGkcC9hAJ-ARcYq_z6lDZV7kT1xD&index=10): add 'edit' & 'delete' in dashboard page.

   
## Installation
- To install and run this project - install dependencies using npm and then start your server:
```
$ npm install
$ npm run dev
```

- (option) VScode EJS language support: beautify the display of EJS
- NodeJs
- Database (MongoDB) Free Cluster (https://www.mongodb.com/) sign up by your Google account. You can reference from Part 4 video.
- after git clone, you have to import all the libraries used in the project under the project folder.
```
npm i bcrypt connect-mongo cookie-parser dotenv ejs express express-ejs-layouts express-session jsonwebtoken method-override mongoose
```
- Also, you need to import nodemon
```
npm i nodemon --save-dev
```


- Create a .env file to store your credentials. After you sign up MongoDB, you can copy a url like below.

```
MONGODB_URI=mongodb+srv://<username>:<password>@clusterName.xxxxxxx.mongodb.net/blog
JWT_SECRET=MySecretBlog
```

- try to run on local. The default port is 5000, but you can change if it is occupied.


## Host on Cyclic
- change the start script in package.json. It should be "node app.js"
```
"scripts": {
    "start": "node app.js",
```
- change the port from 5000 to 3000. (According to the instructon of Cyclic)
```
const PORT = process.env.PORT || 3000;
```
- create an account in Cyclic
- connect your github account with Cyclic.
- get an web url. Check the IP address of the url.
- Paste your MONGODB_URL at the variable page on Cyclic.
- add IP address on MongoDB atlas: including your Cyclic web ip and 0.0.0.0 (connect everywhere)
- It should work.

##MongoDB 

----------------Know more about Raddy-------------
## Design Files
The Blog layout is available in a Figma(.fig) file located under the "Design Files".

[View Live Figma Prototype](https://www.figma.com/proto/Vpc5J1ajnwDTT96q0IUFDJ/NodeJs-Blog?page-id=0%3A1&type=design&node-id=48-119&viewport=-194%2C377%2C0.17&scaling=min-zoom&starting-point-node-id=48%3A119)


### YouTube Channels
[Subscribe to TheNetNinja](https://www.youtube.com/@NetNinja)
[Subscribe to RaddyDev](https://www.youtube.com/@RaddyDev)


### Website
[www.raddy.dev](https://www.raddy.dev)
### Donations
[Buy Raddy a Coffee](https://www.buymeacoffee.com/RaddyTheBrand)
