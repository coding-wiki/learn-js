# Learn ReactJS

React is a JavaScript library for building user interfaces.
https://facebook.github.io/react/

## Contents:
- **React Core**
  - [Component](./component/)
  - []

## Getting Started
- Create a new folder and run these bash commands to set-up the React environment:

  macOS

  ```bash
    npm init -y
    // @0.23.0 @1.0.0 babel-loader@8.0.2
    npm install -s react react-dom webpack@4 webpack-cli@3 webpack-dev-server@3 style-loader css-loader babel-loader  # install webpack, dev server and path
    touch webpack.config.js # create webpack config

    npm install --save-dev @babel/core@7 @babel/cli@7 @babel/preset-env@7 @babel/preset-react@7 # setup babel

    touch .babelrc  # create babel config

    mkdir client
    mkdir client/js
    touch client/js/index.js
    touch client/index.html

    mkdir client/js/components
    touch client/js/components/App.jsx

    bash populate-config.sh

  ```

## Creating an Element
```js
import React from 'react';

class Hello extends React.Component {
  render() {
    return React.createElement('div', null, `Hello ${this.props.name}`);
  }
}

ReactDOM.render(
  React.createElement(Hello, { name: 'World' }, null),
  document.getElementById('root')
);
```

## Resources
- [react-howto README](https://github.com/petehunt/react-howto)
