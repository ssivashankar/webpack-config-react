If it's react app

install below as dependency
react
react-dom 


Below as dev dependency

babel-core
babel-loader
@babel/preset-env or babel-preset-env
@babel/preset-react or babel-preset-react

webpack
webpack-cli
webpack-dev-server
html-webpack-plugin

//Actiual
"devDependencies": {
    "@babel/core": "^7.8.6",
    "@babel/preset-env": "^7.8.6",
    "@babel/preset-react": "^7.8.3",
    "babel-loader": "^8.0.6",
    "html-webpack-plugin": "^3.2.0",
    "webpack": "^4.42.0",
    "webpack-cli": "^3.3.11",
    "webpack-dev-server": "^3.10.3"
  }

Create a file called webpack.config.js

const path = require('path')
const HtmlWebpackPlugin = require('html-webpack-plugin')

module.exports = {
    entry: '',
    output: {

    },
    module: {
        rules: [{
            test:'',
            exclude: '',
            use: {
                loader: ''
            }
        }]
    },
    plugins: []
}

---------------

create .babelrc for presets

{
    "presets": ["env", "react"]
}

---------------

Package JSON

"scripts": {
    start: "webpackdev-server --mode development --open --hot",
    build: "webpack --mode production"
}