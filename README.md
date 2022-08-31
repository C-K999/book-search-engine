# [MERN Challenge: Book Search Engine](https://module-last-bse.herokuapp.com/)

This web application is an attempt to refactor a fully functioning Google Books API search engine built with a RESTful API into a GraphQL API built with Apollo Server. A user can type a search term in a search box and the results will appear.

## Table of Contents

- [Technologies](#technologies)
- [Deployed Link](#link)
- [Usage](#usage)
- [Demo](#demo)
- [Credits](#credits)
- [License](#license)

## Technologies Used

- HTML
- JavaScript
- [MongoDB Atlas](https://www.mongodb.com/cloud/atlas)
- [Heroku](https://www.heroku.com)
- NPM:

1. [Apollo Client Package](https://www.npmjs.com/package/stripe)
2. [Apollo-Server-Express Package](https://www.npmjs.com/package/apollo-server-express)
3. [GraphQL Package](https://www.npmjs.com/package/graphql)
4. [Bcrypt Package](https://www.npmjs.com/package/bcrypt)
5. [Express.js Package](https://www.npmjs.com/package/express)
6. [JSONWebToken](https://www.npmjs.com/package/jsonwebtoken)
7. [Mongoose Package](https://www.npmjs.com/package/mongoose)
8. [Node.js](https://nodejs.org/en/)
9. [nodemon Package](https://www.npmjs.com/package/nodemon)
10. [JWT-Decode Package](https://www.npmjs.com/package/jwt-decode)
11. [React Package](https://www.npmjs.com/package/react)
12. [React-Bootstrap](https://www.npmjs.com/package/react-bootstrap)
13. [React-Dom](https://www.npmjs.com/package/react-dom)
14. [React-Router-Dom](https://www.npmjs.com/package/react-router-dom)
15. [React-Scripts](https://www.npmjs.com/package/react-scripts)

The app was built using the MERN stack, with a React front end, MongoDB database, and Node.js/Express.js server and API.

## Link

[Here.](https://module-last-bse.herokuapp.com/)

## Usage

Simply install the package. Then, on the terminal, run

```
npm install
```

Next, run

```
npm run build
```

And finally, start the server by running

```
npm start
```

## Code Snippet

The following code provides an outlook in how the model functions, taken from `/server/schemas/typeDefs.js` where the various objects from `/models` are defined and typed.

```
type User {
    _id: ID!
    username: String!
    email: String!
    bookCount: Int
    savedBooks: [Book]
  }
  type Book {
    bookId: String!
    authors: [String]
    description: String
    title: String!
    image: String
    link: String
  }
  type Auth {
    token: ID!
    user: User
  }
```

## Demo

Here's a screenshot of the web application.

![default](/media/demo.png)

And here is a demonstration of the web application in action, where a vareity of titles are searched.

![action](/media/demo.gif)

Within the `/media` directory, there's also a video demonstration.

## Developer Information

### **Clement Koo**

[LinkdIn](https://www.linkedin.com/in/clement-t-k-459322138/) |
[GitHub](https://github.com/C-K999)

## Credits

UCB - Coding Bootcamp

---

© 2022 Clement Koo. All Rights Reserved.
