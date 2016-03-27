# Badass React Snippets [![Build Status](https://travis-ci.org/tylerbuchea/badass-react-snippets.svg?branch=master)](https://travis-ci.org/tylerbuchea/badass-react-snippets)
**Package for Github's Atom Editor**

## About
These snippets are made to work with the latest ES6 standards, adhere to the [airbnb eslint config](https://github.com/airbnb/javascript/tree/master/packages/eslint-config-airbnb), and are React/React-Native agnostic.

**Add the airbnb config to your project (optional)**
```
npm install --save-dev eslint-config-airbnb babel-eslint eslint-plugin-react eslint
echo '\''{ extends: [airbnb], }'\'' > .eslintrc'
```

## Installation

``` bash
apm install badass-react-snippets
```

## Usage
After install just type one of the titles below and hit tab then the snippet will expand in your editor. Only works on files already saved as `.js` or `.jsx`

Continue hitting tab to cycle through and highlight common editing points in a snippet. The `${N}` syntax in the examples below denote the highlight points.

## rcc
**React ES6 Component with Constructor**

``` javascript
import React, {
  PropTypes,
} from 'react${2:-native}';

export default class ${1:MyComponent} extends React.Component {
  constructor(props) {
    super(props);
  }

  render() {
    return (
      ${3:<View></View>}
    );
  }
}

${1}.propTypes = {
  style: PropTypes.number,
};
```

## rc
**React ES6 Component**

``` javascript
import React, {
  PropTypes,
} from 'react${2:-native}';

export default class ${1:MyComponent} extends React.Component {
  render() {
    return (
      ${3:<View></View>}
    );
  }
}

${1}.propTypes = {
  style: PropTypes.number,
};
```

## rfunc
**React ES6 Functional Component**

``` javascript
import React, {
  PropTypes,
} from 'react${2:-native}';

export function ${1}(props) {
  return (
    ${3:<View></View>}
  );
}

${1}.propTypes = {
  style: PropTypes.number,
};
```

## rconst
**React ES6 Constructor**

``` javascript
constructor(props) {
  super(props);
  ${1}
}
```

## rbm
**React ES6 bind method to this**

``` javascript
this.${1} = this.${1}.bind(this);
```
