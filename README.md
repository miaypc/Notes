# Node.js
Node.js is an open source, cross-platform, Javascript runtime environment, optimised for scalability with many input/output operations (wikipedia).

## Modules
### module.exports lets you expose code to the rest of the application.
```
module.exports = () => {
  const message = "Hello World";
  console.log(message);
}
```
### The require statement allows to "load" an external module by specifying the file path.
```
const helloworld = require('./hello');
```
### HTTP module
http.createServer() takes a function as a parameter that will be called for each connection to the server.

listen() listens for incoming connections on port 3000.
```
const http = require('http');

const server = http.createServer((request, response) => {
    response.writeHead(200);
    response.end('Hello World');
});

server.listen(3000);
console.log('Server address: http://localhost:3000');
```

## npm
NPM and Yarn are different package managers but they both get their packages from the NPM registry.
### Creates the package.json file 
```
$ npm init
```
### install dependencies(locally)
```
 npm install package_name --save
```
### install dependencies(globally)
``` 
npm install package_name --save -g
```

### .gitignore
.gitignore is a special file used by git where you can specify files and folders that you want to keep out of the GIT repository.

### Package.json
```
 "devDependencies": {},
  "scripts": {
    "start": "node main.js",
    "sample": "echo “Sample” && node main.js"
  },
```
# React
What is React?
React is a way to build user interfaces. It is only concerned with what you see on the front-end. React makes user interfaces very easy to build by cutting each page into pieces. We call these pieces components.

### Components
A React component is a bit of code that represents a piece of the page. Each component is a JavaScript function that returns a piece of code that represents a piece of a web page.
![Image of components](https://github.com/miaypc/Notes/blob/master/images/components.png)

### props & stats
State can be changed (Mutable)
Whereas Props can't (Immutable)

![Image of props and state](https://github.com/miaypc/Notes/blob/master/images/propsandstate.png)

###  State
State is way to update our UI based on events.
```
class Card extends React.Component {
  constructor(props) {
    super(props);
    this.state = {
      bg: "pink"
    };
  }
 ```
A constructor method of a React component always needs to call super(props) before anything else.
we have an object representing our components state.In the render function, this is always referring to the component it is within.

```
changeColor = () => {
    this.setState({ bg: "grey" });
  };
```
We can change state with this.setState(), if we give it a new object representing the new state.
When we change the state of our component, it will call the render function again.

### Importing a Component
```
import React from "react";
import "./index.css";
import Card from "@material-ui/core/Card";
```


