
## How to passing children in React
export default function App() {
  return (
    <div className="App">
      <Example header={<h1>hello</h1>}>
        <h2>world</h2>
        <p>!!!!</p>
      </Example>
    </div>
  );
}

import React from "react";

function Example({ children, header }) {
  return (
    <div>
      {header}

      {children}
    </div>
  );
}

export default Example;



## What is a DB model?
#### A database model describes how data can be stored, organized and accessed in a database.

## What is a Relational DB model?
#### A Relational db Model is the type of database model that describes Relational Databases.
#### It describes all the tables, relations between the tables and data constraints.

There are 3 types of relations:

one-to-one

one-to-many

many-to-many

![Image of props and state](https://github.com/miaypc/Notes/blob/master/images/database.png)

