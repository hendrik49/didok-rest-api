# Express REST API - Node.JS 

Structure for node.js projects involving typescript

### Prerequisites

In order to use this project, you must have the following requirements:

* NODE
* NPM

### Structure

Project structure:
```
├── src
│   ├── api               ---> The Folder to handler API layers
│   │   ├── controllers   ---> Input and Output of the application, along with basic request validations.
│   │   │
│   │   ├── middlewares   ---> Request Interceptors
│   │   │
│   │   └── routes        ---> App route settings
│   │
│   ├── config            ---> Application Settings, Logging, Environment, Express middleware ...
│   │
│   ├── interfaces        ---> Implementation of interfaces for development assistance
│   │
│   ├── models            ---> Models, Entities and Schemas for manipulation and persistence.
│   │
│   ├── persistence       ---> Definitions and database instances.
│   │
│   └── services          ---> It gathers business rules and external manipulations (Database, other api's ...)
│
├── tests                 ---> Unit Tests

```

### Installing and Running

So you can run your project in your environment, follow these steps:

Clone the project in your preferred folder.


```
cd nodejs-rest-api
```

```
npm install
```

```
npm run dev
```

And ready! The application will be running on the port defined in src/server.ts

## Running the tests

This application has unit tests using the [Jest](https://jestjs.io/) framework.

To run unit tests:

```
npm run test
```

To run unit tests with coverage:

```
npm run coverage
```


### And coding style tests

So that we can write cleaner and more beautiful code, we can adopt linear frameworks like [Eslint](https://eslint.org/).

```
npm run lint
```

## Deployment


If you want to enjoy the application in production, you can use the [Docker](https://www.docker.com/).

For this, the project has the Dockerfile configuration file, so that it can generate the project image.

```
docker build --name nodejs-api .
```

```
docker run -d -p 8080:8080 nodejs-api
```

## Built With

* [Express](https://expressjs.com/pt-br/) - The web framework used
* [TypeScript](https://www.typescriptlang.org/) - Is a Typed superset of Javascript
* [Mongoose](https://mongoosejs.com/) - Elegant mongodb object modeling for node.js
* [Jest](https://jestjs.io/) - Is a delightful JavaScript Testing Framework
* [Eslint](https://eslint.org/) - The pluggable linting utility for JavaScript
* [EditorConfig](https://editorconfig.org/) - Helps maintain consistent coding styles

## References

* [Santiq](https://softwareontheroad.com/ideal-nodejs-project-structure/?utm_source=devto&utm_medium=post) - Bulletproof node.js project architecture
* [RocketSeat](https://github.com/Rocketseat/youtube-typescript-nodejs) - Project code produced during TypeScript video on NodeJS