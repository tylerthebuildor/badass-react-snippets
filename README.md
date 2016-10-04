# Badass React Snippets [![Build Status](https://travis-ci.org/tylerbuchea/badass-react-snippets.svg?branch=master)](https://travis-ci.org/tylerbuchea/badass-react-snippets)
**Package for Github's Atom Editor**

## About
These snippets are made to work with the latest ES6 standards, adhere to the [airbnb eslint config](https://github.com/airbnb/javascript/tree/master/packages/eslint-config-airbnb), and are React/React-Native agnostic.

**Add the airbnb eslint config to your project (optional)**
```
npm install --save-dev eslint eslint-config-airbnb eslint-plugin-import eslint-plugin-react eslint-plugin-jsx-a11y
echo '\''{ extends: [airbnb], }'\'' > .eslintrc'
```

## Installation

``` bash
apm install badass-react-snippets
```

## Usage
After install just type one of the titles below and hit tab then the snippet will expand in your editor. Only works on files already saved as `.js` or `.jsx`

Continue hitting tab to cycle through and highlight common editing points in a component.

## rcc
**React ES6 Component with Constructor**

``` jsx
import React, {
  Component,
  PropTypes,
} from 'react';

import {
  View,
} from 'react-native';

const propTypes = {};

const defaultProps = {};

export default class MyComponent extends Component {

  constructor(props) {
    super(props);
    this.state = {};
  }

  render() {
    return (
      <div>
        <h1>Title</h1>
      </div>
    );
  }

}

MyComponent.propTypes = propTypes;
MyComponent.defaultProps = defaultProps;

```

## rc
**React ES6 Component**

``` jsx
import React, {
  Component,
  PropTypes,
} from 'react';

import {
  View,
} from 'react-native';

const propTypes = {};

const defaultProps = {};

export default class MyComponent extends Component {

  render() {
    return (
      <div>
        <h1>Title</h1>
      </div>
    );
  }

}

MyComponent.propTypes = propTypes;
MyComponent.defaultProps = defaultProps;

```

## rfunc
**React ES6 Functional Component**

``` jsx
import React, {
  PropTypes,
} from 'react';

import {
  View,
} from 'react-native';

const propTypes = {};

const defaultProps = {};

export default function MyComponent(props) {
  return (
    <div>
      <h1>Title</h1>
    </div>
  );
}

MyComponent.propTypes = propTypes;
MyComponent.defaultProps = defaultProps;

```

## rconst
**React ES6 Constructor**

``` jsx
constructor(props) {
  super(props);
  this.state = {
    someVariable,
  };
}
```

## rbm
**React ES6 bind method to this**

``` jsx
this.someMethod = this.someMethod.bind(this);
```

## rcc7
**React ES7 Component with Constructor using static. Not airbnb compliant.**

``` jsx
import React, {
  Component,
  PropTypes,
} from 'react';

import {
  View,
} from 'react-native';

export default class MyComponent extends Component {

  static defaultProps = {}

  static propTypes = {}

  constructor(props) {
    super(props);
    this.state = {};
  }

  render() {
    return (
      <div>
        <h1>Title</h1>
      </div>
    );
  }

}

```
