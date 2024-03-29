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

# Create React App Conventions

- Good style: each react component goes in separate file
  - src/Car.js for Car component
  - src/House.js for House component

name of file should match name of the component;
should be capitalized

- components should extends Componenet (imported from React)

  - export the component as the default object

- skeleton assumes top object is App in App.js
  - best to keep this

# Assets and CRA - like CSS and images

to include images and CSS, you can import them in JS files

# CSS

- make the CSS file the same name as each React component
  - House.css for House componenet
- import it at the top of House.js

  - create-react-app will automatically load that CSS

- conventional to add 'className="House"' onto House div

  - and use that as prefix for sub-items to style:

  ```
  <div className="House" >
   <p className="House-title">{this.props.title}</p>
    <p className="House-address">{this.props.addr}</p>
  ```

# Images

- store images in src/folder with the components
- load them where needed, and use imported name where path should go:

```
import puppy from "./puppy.jpg";

class Animal extends React.Component {
  render() {
    return(
      <div>
      <img src={puppy} alt="Cute puppy!" />
      </div>
    )
  }
}
```
