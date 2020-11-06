# React with Webpack
> Create a React application manually with webpack

 <img src="webpack-logo.png" width="250">

Though it is painless to get started with create-react-app to make your own React application, it is however beneficial in some cases to manually configure your own application. 'create-react-app' does a lot of things for you which may or may not meet the needs of your project. So knowing how to configure your own React application can come in handy.


## Installation

Install and get this project up and running just like any other React application

```bash
npm install
npm start
```

Notice that in `package.json`, the scripts for building and starting the application use the `webpack` instead of the traditional `react-scripts`.

## Configuration

This application has been configured the following way through the `webpack.config.js` file:

-  It's entry point is the file `index.js`
- The output of build is minified and stored in `main.js`
- It has an integrated `devServer` that runs on the port 3000 and has `hot` enabled which allows live reloading
- It has a `source-map` devtool integrated which will allow easy debugging of the application in case of errors from browser Dev Tools. For example, without `source-map`, you might not be able to trace the line causing error from the browser inspection panel. It will give you an unfamiliar snippet of code. `source-map` fixes this and shows you your familiar code inside the browser console.
- It has a few `rules` integrated such as loaders for `babel`, which will eventually transpile all code to `JavaScript` so it can be displayed in the browser. This allows you to code using `ES6` or `TypeScript`. Similarly, we have a `CSS` loader to transpile `CSS` or `SCSS` code. 

There are numerous rules that you can set in this configuration file to meet your organizational and personal needs for the project.