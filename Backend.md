# Backend ---Todo List

## Create the most basic skeleton

#### 1. create the folders and server.js inside Back
   ![Image](https://github.com/miaypc/Notes/blob/master/images/backend-one.png)

#### 2. Terminal --in Back: 
   npm init -y
   yarn add mongoose
   yarn add -D nodemon
   yarn add express
   
#### 3. in server.js
   ![Image](https://github.com/miaypc/Notes/blob/master/images/backend-two.png)

#### 4. in package.json:
   under "scripts" add:
  "dev": "nodemon server.js"

#### 5. in terminal:
   yarn dev
   
 #### 6. in postman:
   ![Image](https://github.com/miaypc/Notes/blob/master/images/backend-three.png)

## Connect with Mongo

#### 1. in server.js
   ![Image](https://github.com/miaypc/Notes/blob/master/images/backend-four.png)

#### 2.define model:
   #### inside models, create todo.model.js
   ![Image](https://github.com/miaypc/Notes/blob/master/images/backend-five.png)
   
  ##### in todo.model.js (creating the table)
   ![Image](https://github.com/miaypc/Notes/blob/master/images/backend-six.png)
   
## Create-Post
   
#### 1.create functions
   #### inside services, create todo.services.js
   ![Image](https://github.com/miaypc/Notes/blob/master/images/backend-8.png)
   
   ![Image](https://github.com/miaypc/Notes/blob/master/images/backend-9.png)
   
#### 2.create controllers
   #### inside controllers, create todo.controller.js
   ![Image](https://github.com/miaypc/Notes/blob/master/images/backend-10.png)
   
   ![Image](https://github.com/miaypc/Notes/blob/master/images/backend-11.png)
   
#### 3.create routes
   #### inside routes, create todo.model.js
   ![Image](https://github.com/miaypc/Notes/blob/master/images/backend-7.png)
   
   ![Image](https://github.com/miaypc/Notes/blob/master/images/backend-12.png)
   
#### 4.Check in Postman
   ![Image](https://github.com/miaypc/Notes/blob/master/images/backend-13.png)
 


