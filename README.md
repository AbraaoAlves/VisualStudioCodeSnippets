# Visual Studio Code Snippets
Snippets for [Visual Studio Code](https://code.visualstudio.com/)

## How to configure snippets on VSCode

To enable these snippets in Visual Studio Code, press Ctrl+Shift+P and type snippets. 
Hit enter on ```Preferences: Snippets```, then choose the language.

If you chose JavaScript, the javascript.json file will open. Just add snippets for ```.js``` files here. 

## Javascript

All JavaScript snippets are in [javascript.json](https://github.com/danilojrr/VisualStudioCodeSnippets/blob/master/javascript.json) file.

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

## JSX

All JSX snippets are in [javascriptreact.json](https://github.com/danilojrr/VisualStudioCodeSnippets/blob/master/javascriptreact.json) file.

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