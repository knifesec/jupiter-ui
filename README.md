# Neptune :blue_heart::alien::fire::guitar::tada:

Neptune is a Component library written in ReactJs and Sass with a fresh and new style.
The main scope of the library is to give to users a project ready library of graphical components to speed up their work and worry only of the logic and layout of the applications.

# Components

We try to provide two versions of the components.
One uses the standard 2.0 material design (all rewrittenby us in a React way).
The other uses a fresh design thinked and designed by us.

# Installation

All you need todo is to run this command to add to your ReactJs and Sass project Neptune:

    npm install --save @neptune

# Getting Started

### Create a react project

The simpliest and best way to create a standard react project is to use the great `create-react-app` packages
Installaiton:

    npm install -g create-react-app

> NOTE: To run this command you need to install node and npm to your pc
> You can use npm as well as yarn
> create-react-app repo: https://github.com/facebook/react

Now you can create your project:

    create-react-app your-project-name
    cd your-project-name
    npm install

Ok, if no error are occurred running those commands you can run `npm start` to run your new project to a local web server visible in the browser at `localhost:3000`

The next step is to install the scss compiler to CSS:

    npm install --save-dev node-sass-chockidar npm-run-all

after this in the `package.json` replace these lines:

    "scripts": {
    	  "start": "react-scripts start",
    	  "build": "react-scripts build",
    	  "test": "react-scripts test --env=jsdom",
    	  "eject": "react-scripts eject"
    }

with:

    "scripts": {
    	  "build-css": "node-sass-chokidar --include-path ./src --include-path ./node_modules 									./src/App.scss -o ./src",
    	  "watch-css": "npm run build-css && node-sass-chokidar --include-path ./src --include-path ./node_modules --watch ./src/App.scss ./src/App.css",
    	  "start-js": "react-scripts start",
    	  "start": "npm-run-all -p watch-css start-js",
    	  "build-js": "react-scripts build",
    	  "build": "npm-run-all build-css build-js",
    	  "test": "react-scripts test --env=jsdom",
    	  "eject": "react-scripts eject"
    }

now you can write all your awesome code!! this is an example:

    import React, {Component} from 'react';
    import Button from '@material/react-button/dist'; // /index.js is implied

    import './App.css';
    // add the appropriate line(s) in Step 2a if you are using compiled CSS instead.

    class App extends Component {
    	render() {
        return (
          <div>
            <button>ciao!!!</button>
          </div>
        );
      }
    }

    export default App;

> Rename your App.css file to App.scss
> NOTE if you don't use scss you can skip all the scss configuration

## We need your help!!!

This project is an completely open project made in our free times, is not a "company" project. So don't esistate to help and contributing!!! You can contact us by **Gitter**

## License

This project is under MIT License
