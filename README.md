# Badass React Snippets
**Package for Github's Atom Editor**

## Installation

``` bash
git clone https://github.com/tylerbuchea/badass-react-snippets

# Enter cloned folder

apm link
```

After install just type one of the titles below and hit tab then the snippet will expand in your editor. Only works on files already saved as `.js`


## rcc

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

``` javascript
constructor(props) {
  super(props);
  ${1}
}
```
