## amazona

## Introduction

Basic ecommerce app that allows users to shop for clothes. Built using MongoDB, Express.js, React.js, Redux, and Node.js (MERN stack).

This project was part of a [Udemy](https://www.udemy.com/course/build-ecommerce-website-like-amazon-react-node-mongodb/) course.

### Setup

* In the root directory, rename .env.example to .env and add your MONGODB_URL.

* To add example products to the database:

    1) Uncomment lines 4 and 8-15 in routers/productRouter.js.

    2) Go to http://localhost:5000/api/products/seed.

* This project is in the Paypal [sandbox](https://developer.paypal.com/tools/sandbox/) environment. To use live Paypal accounts, add a PAYPAL_CLIENT_ID to your .env file.

* Install dependencies

```
# Backend dependencies
npm install

# Frontend dependencies
cd frontend
npm install
```

### Run development environment

In the project root directory

```
npm run dev
```

### Deploy to Heroku

Setup repository

```
git init

git add .

git commit -m "initial commit"

git branch -M main
```

Create a new empty application on heroku and push code

```
heroku create

git push heroku main:master
```

Set heroku environment variables

```
heroku config:set MONGODB_URL=YOUR_MONGO_URL
```

Open application

```
heroku open
```

### Demo

https://ia-mern-amazona.herokuapp.com