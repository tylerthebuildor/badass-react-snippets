# Badass React Snippets [![Build Status](https://travis-ci.org/tylerbuchea/badass-react-snippets.svg?branch=master)](https://travis-ci.org/tylerbuchea/badass-react-snippets)
**Package for Github's Atom Editor**

## Installation

``` bash
git clone https://github.com/tylerbuchea/badass-react-snippets
cd badass-react-snippets
apm link
```

After install just type one of the titles below and hit tab then the snippet will expand in your editor. Only works on files already saved as `.js`


## rcc
**React ES6 Component**

``` javascript
import React, {
  PropTypes,
} from 'react';

export default class ${1:MyComponent} extends React.Component {
  constructor(props) {
    super(props);
  }

  render() {
    return (
      ${2:<View></View>}
    );
  }
}

${1}.propTypes = {
  style: PropTypes.number,
};
```

## rc
**React ES6 Component with Constructor**

``` javascript
import React, {
  PropTypes,
} from 'react';

export default class ${1:MyComponent} extends React.Component {
  render() {
    return (
      ${2:<View></View>}
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
} from 'react';

export function ${1}(props) {
  return (
    ${2:<View></View>}
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
