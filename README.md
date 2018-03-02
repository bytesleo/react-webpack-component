
# react-webpack-component

[![NPM version](https://badge.fury.io/js/react-webpack-component.svg)](https://npmjs.org/package/react-webpack-component) [![GitHub license](https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat-square)](https://raw.githubusercontent.com/kevoj/role-calc/master/LICENSE)

> Base structure in Webpack 4 for the creation of npm modules in React

### Installation

**1. Clone**

```bash
git clone https://github.com/kevoj/react-webpack-component.git your-react-component-name
cd [your-react-component-name]
npm install
```
**2. Set name of the library**

Replace in **package.json**

```json
{
    "name": "your-react-component-name",
    ...
}
```
**3. Create Link**

```bash
npm run build
npm link
```

## Development

### Start

Watch changes in mode development

```bash
npm start
```

### Build

Compile in mode production

```bash
npm run Build
```
### Structure

<pre> 
|-- dist (Compiled)
|   `-- index.js
|-- src (Your code here, view example in code source...)
|   |-- components
|   `-- index.js
`-- webpack.config.js
</pre> 

### Test the component in a project

```bash
cd Existing-React-Project
npm link your-react-component-name
```

### At this point you can already use your component, usage:

```javascript
import React, { Component } from 'react';
import { Example } from 'your-react-component-name'

class HelloWorld extends Component {
  render() {
    return (
        <Example />
    );
  }
}
export default HelloWorld;
```

## Production

### Publish in NPM

**1. Compile to production**

```bash
npm run build
```

**2. Login**

```bash
npm login
# login with your credentials in https://www.npmjs.com/
```

**3. Upload package**

**Note:** Verify your version of the component in **package.json**, you can not upload the same version twice

```bash
npm publish
# Available in https://www.npmjs.com/package/your-react-component-name
```
Now, you can install your package with:

```bash
npm install your-react-component-name--save
# :)
```

## License

MIT © [Leonardo Rico](https://github.com/kevoj/react-webpack-component/blob/master/LICENSE)