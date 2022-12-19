# FullStack Social Media App
Complete React MERN Full Stack Social Media App


For users who are looking to contribute, I'm planning to possibly create a separate branch for community contributions and additional features as well as for improvements and fixes.

I haven't decided on the exact workflow I'll be using yet. But we'll get it out there soon!

## Notes for YouTube video
- https://youtu.be/K8YELRmUb5o

### [0:00]  Build a Fullstack MERN React Responsive Social Media Application from Scratch

M - Mongo
E - Express
R - React
N - Node.js

images from https://unsplash.com/

#### download and install node from https://nodejs.org/en/
```
node -v
v16.14.0
```

#### install dependencies
```
$ npm i -g nodemon  # dev server refresh immediately after code change

$ npm i express body-parser bcrypt cors dotenv gridfs-stream multer multer-gridfs-storage helmet morgan jsonwebtoken mongoose

npm audit fix --force

npm init -y

```

#### install npx - node runtime
```
npm i -g npx
npx -v
8.13.1
```

#### install IDE - VS Code

Extensions: Prettier Format, SmartSemicolon

#### setup backend server layout

#### signup Mongodb

see \fullstack\my-sciomedia\server\docs\sociopedia-app.png

Install MongoDB Compass

connect str = mongodb+srv://<username>:<password>@cluster0.xntq7hf.mongodb.net/test

### [5:07] Backend Installation of Node, Visual Studio Code, and Backend Packages

### [7:44] Backend Configurations and Middleware Setup

### [16:06] MongoDB Registering, Installation and Setup

### [21:31] Data Modeling and ERD Diagrams
see \fullstack\my-sciomedia\server\docs\data-model.png

### [26:08] Authentication and Authorization in Node

\server\routes\auth.js
\server\controllers\auth.js  # for authentication
\server\middleware\auth.js   # for authorization

### [59:07] User Routes Setup

\server\models\User.js
\server\routes\users.js
\server\controllers\users.js

### [1:13:33] Post Routes Setup

\server\models\Post.js
\server\routes\posts.js
\server\controllers\posts.js

### [1:36:20] Backend Data Add and Demo

Mock data:  \server\data\index.js

cd server
node index.js

### [1:42:20] Frontend Installation and Setup
```
npx create-react-app client  # CRA
cd client

npm i react-redux @reduxjs/toolkit redux-persist react-dropzone dotenv formik yup react-router-dom @emotion/react @emotion/styled @mui/material @mui/icons-material

npm audit fix --force

```

cleanup src/App.js

get Fonts `Rubik` 400/500/700 at fonts.google.com


```
npm start
```

### [1:48:34] React Redux File Folder Architecture and React Router

### [1:56:10] Redux and Toolkit Installation and Setup

manage app states:
src/state/index.js


### [2:10:56] Color, Theme, Dark Mode, and Styling Setup



### [2:26:16] Navbar

### [2:48:37] Register, Login Pages, and Form

Form is a big component

### [3:34:44] Home Page and Widgets

### [4:04:17] Posts and Post Widgets

### [5:19:41] Profile Page

### [5:27:08] Full Stack MERN React Application Complete


### Finally

To run the app
```
cd server
node index.js   # server_url = http://localhost:3001

cd client
npm start
```

## Features + Issues

- implement `Search`
- implement `Share` button
- friends array should not allow self (or parent user)
when adding friend from PostFeed, ensure post.userId <> userId

- implement `Add comment`

- implement Clip, Attachment, Audio post (besides description and image)

- limit total number posts to fetch to avoid performance issue

- `FlexBetween` should be called `StyledBox`

## Credits

### Thank You, EdRoh is my hero!

Material UI: https://mui.com/material-ui/getting-s...
Redux Toolkit: https://redux-toolkit.js.org/introduc...
React Router: https://reactrouter.com/en/v6.3.0/get...
Redux Persist: https://github.com/rt2zz/redux-persist
React Dropzone: https://react-dropzone.js.org/
Node: https://nodejs.org/en/download/
Nodemon: https://github.com/remy/nodemon
NPX: https://www.npmjs.com/package/npx
VsCode: https://code.visualstudio.com/download
Dotenv: https://github.com/motdotla/dotenv
MongoDB: https://www.mongodb.com/
Mongoose: https://github.com/Automattic/mongoose
JsonWebToken: https://github.com/auth0/node-jsonweb...
Multer: https://github.com/expressjs/multer
GridFS-Storage: https://github.com/devconcept/multer-...
Google Fonts: https://fonts.google.com/
Formik: https://formik.org/docs/overview
Yup: https://github.com/jquense/yup

completed code: https://github.com/ed-roh/mern-social...
assets file: https://github.com/ed-roh/mern-social...
input data file: https://github.com/ed-roh/mern-social...
theme file: https://github.com/ed-roh/mern-social...