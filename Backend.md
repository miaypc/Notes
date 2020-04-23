## Backend ---Todo List

### create the most basic skeleton
1. create the folders and server.js inside Back
![Image of one](https://github.com/miaypc/Notes/blob/master/images/backend-one.png)

2. Terminal --in Back: 
   npm init -y
   yarn add mongoose
   yarn add -D nodemon
   yarn add express
   
3. in server.js
![Image of one](https://github.com/miaypc/Notes/blob/master/images/backend-two.png)

4. in package.json:
   under "scripts" add:
  "dev": "nodemon server.js"

5. in terminal:
   yarn dev
   
 6. in postman:
 ![Image of one](https://github.com/miaypc/Notes/blob/master/images/backend-three.png)

### connect with Mongo
1. in server.js
![Image of one](https://github.com/miaypc/Notes/blob/master/images/backend-four.png)

2. define model:
   inside models, create todo.model.js
   ![Image of one](https://github.com/miaypc/Notes/blob/master/images/backend-five.png)
   
   in todo.model.js (creating the table)
   ![Image of one](https://github.com/miaypc/Notes/blob/master/images/backend-six.png)


