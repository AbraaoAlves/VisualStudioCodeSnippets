# Visual Studio Code Snippets
Snippets for [Visual Studio Code](https://code.visualstudio.com/)

## Snippets for

* [JavaScript](#javascript)
* [JSX & React](#jsx)

## Configuration

To enable these snippets in Visual Studio Code, press Ctrl+Shift+P and type snippets. 
Hit enter on ```Preferences: Snippets```, then choose the language. It'll open a .json file.

For example, if you choose JavaScript, the javascript.json file will open. Now, just add some snippets from our [javascript.json](https://github.com/danilojrr/VisualStudioCodeSnippets/blob/master/javascript.json) into your javascript.json. 

## Javascript

Follow [Configuration](#configuration) steps to open the javascript.json file in your VS Code. 

JavaScript snippets available [here](https://github.com/danilojrr/VisualStudioCodeSnippets/blob/master/javascript.json).

### [im] Import statement

```javascript
import ${variableName} from '${path}';
```

### [re] Require statement

```javascript
require('${path}');
```

### [lt] let variable

```javascript
let ${variableName} = ${value};
```

### [ct] constant variable

```javascript
const ${VARIABLE_NAME} = ${value};
```

### [cls] Class with empty body

```javascript
class ${ClassName} {
    $0
}
```

### [clsc] Class with constructor

```javascript
class ${ClassName} {
    constructor(${parameters}) {
        $0
    }
}
```

### [clse] Class that extends another class 

```javascript
class ${ClassName} extends ${AnotherClassName} {
    constructor(${parameters}) {
        super(${parameters});
        $0
    }
}
```

### [ctor] Class constructor 

```javascript
constructor(${parameters}) {
    $0
}
```

### [fn] Function

```javascript
function ${name}(${parameters}) {
    $0
}
```

### [afn] Anonymous function

```javascript
function (${parameters}) {
    $0
}
```

### [sw] Switch

```javascript
switch (${variable}) {
    case ${value}:
        $0
        break;
    default:
        return $1;
}
```

### [us] use strict

```javascript
'use strict';
```

### [de] debugger

```javascript
debugger;
```

### [cl] console.log

```javascript
console.log(${value});
```

## JSX & React

Follow [Configuration](#configuration) steps to open the javascriptreact.json file in your VS Code.

JSX snippets available [here](https://github.com/danilojrr/VisualStudioCodeSnippets/blob/master/javascriptreact.json).

__Note 1:__ all JavaScript snippets are included in JSX files.

__Note 2:__ these snippets focuses on ES6 syntax.

### [rc] React component 

```javascript
import React, { Component, PropTypes } from 'react';

export default class ${ComponentName} extends Component {
    constructor(props) {
        super(props);
        
        this.state = {
            ${property}: ${value}
        };
    }
    
    render() {
        return (
            $0
        );
    }
}

${ComponentName}.propTypes = {
    ${propName}: PropTypes.${type}
};
```