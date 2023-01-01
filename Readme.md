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

# Modules: Import and Exports

- Modules
  CRA uses ES2015 "modules"; this is a newer standardized version of Node's require()

You use this to export/import classes/data/functions between JS files

a way of sharing code functions objects classes between JS files

# To Default Export or Not?

- conventionally, defualt exports are used when there's a most-likely thing to export
- e.g. in a react component file, its common to have the component be the default export
- you never need to make a default export, but it can be helpful to indicate the most important thing in a file
