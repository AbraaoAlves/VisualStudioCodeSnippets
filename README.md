# Visual Studio Code Snippets
Snippets for [Visual Studio Code](https://code.visualstudio.com/)

## How to configure snippets on VSCode

To enable these snippets in Visual Studio Code, press Ctrl+Shift+P and type snippets. 
Hit enter on ```Preferences: Snippets```, then choose the language.

If you chose JavaScript, the javascript.json file will open. Just add snippets for ```.js``` files here. 

## Javascript Snippets

All JavaScript snippets are in [javascript.json](https://github.com/danilojrr/VisualStudioCodeSnippets/blob/master/javascript.json) file.

### [im] Import statement

```javascript
import ${variableName} from '${path}';
```

### [re] Require statement

```javascript
require('${path}');
```

### [let] let variable

```javascript
let ${variableName} = ${value};
```

### [const] constant variable

```javascript
const ${VARIABLE_NAME} = ${value};
```

### [class] Class with empty body

```javascript
class ${ClassName} {
    $0
}
```

### [classc] Class with constructor

```javascript
class ${ClassName} {
    constructor(${parameters}) {
        $0
    }
}
```

### [classe] Class that extends another class 

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
        $1
        return;
}
```

### [cl] console.log

```javascript
console.log(${value});
```

### [de] debugger

```javascript
debugger;
```