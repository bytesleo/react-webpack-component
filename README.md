
# react-webpack-component

[![NPM version](https://badge.fury.io/js/react-webpack-component.svg)](https://npmjs.org/package/react-webpack-component) [![Build Status](https://travis-ci.org/kevoj/react-webpack-component.svg?branch=master)](https://travis-ci.org/kevoj/react-webpack-component) [![dependencies Status](https://david-dm.org/kevoj/react-webpack-component/status.svg)](https://david-dm.org/kevoj/react-webpack-component) [![devDependencies Status](https://david-dm.org/kevoj/react-webpack-component/dev-status.svg)](https://david-dm.org/kevoj/react-webpack-component?type=dev)
[![GitHub license](https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat-square)](https://raw.githubusercontent.com/kevoj/role-calc/master/LICENSE)

> Base structure in Webpack for the creation of npm modules in React

### Installation

* **Clone**

```bash
git clone https://github.com/kevoj/react-webpack-component.git
cd react-webpack-component
npm install
```

* **Create Link**

```bash
npm run build
npm link
```

### Start

```bash
npm start
```

### Build

```bash
npm run Build
```

### Structure

<pre> 
|-- build (Compiled)
|   `-- index.js
|-- src (Your code here, view example in code source...)
|   |-- components
|   `-- index.js
`-- webpack.config.js
</pre> 

### Test the component in a project

```bash
mkdir new-project (React project)
cd new-project
npm link react-webpack-component
```

### At this point you can already use your component, usage:

```javascript
import React, { Component } from 'react';
import { Example } from 'react-webpack-component'

class HelloWorld extends Component {
  render() {
    return (
        <Example />
    );
  }
}
export default HelloWorld;
```

## License

MIT © [Leonardo Rico](https://github.com/kevoj/react-webpack-component/blob/master/LICENSE)