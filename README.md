# NodeJs, Express, EJS & MongoDB Blog - CRUD

This repo is used for learning to building a NodeJs blog and how to run it on a free host. I am really appreciate Raddy's efforts for the 10 videos and open source code. 

## Video playlists:
1. 


## Installation
To install and run this project - install dependencies using npm and then start your server:

```
$ npm install
$ npm run dev
```

## You need:
- NodeJs
- Database (MongoDB) Free Cluster (https://www.mongodb.com/) sign up by your Google account
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
