# Create React App

- a utility script that
  - creates a skeleton react project
  - sets it up so that JS files are run through Babel automatically
  - lets us use modern javascript features/idioms
  - makes testing and deployment much easier

required dependencies include:

- node (nodejs.org)

in terminal:

```
npx create-react-app my-app *app name*
cd my-app
npm start (or yarn start)

```

# Creating a new app

# Webpack

- CRA is built on top of "webpack", a JS utility that:

* enables module importing/exporting
* packages up all CSS/images/JS into a single file for browser
* dramatically reduces # of HTTP requests for performance
* hot reloading: when you change a source file, automatically reloads
  - is very clever and tries to only reload relevant files
* enables easy testing and deployment
