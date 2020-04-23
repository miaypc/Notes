# Todo List

# Back

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

#### 2. define model:
   #### inside models, create todo.model.js
   ![Image](https://github.com/miaypc/Notes/blob/master/images/backend-five.png)
   
  ##### in todo.model.js (creating the table)
   ![Image](https://github.com/miaypc/Notes/blob/master/images/backend-six.png)
   
## Create-Post
   
#### 1. create functions
   #### inside services, create todo.services.js
   ![Image](https://github.com/miaypc/Notes/blob/master/images/backend-8.png)
   
   ![Image](https://github.com/miaypc/Notes/blob/master/images/backend-9.png)
   
#### 2. create controllers
   #### inside controllers, create todo.controllers.js
   ![Image](https://github.com/miaypc/Notes/blob/master/images/backend-10.png)
   
   ![Image](https://github.com/miaypc/Notes/blob/master/images/backend-11.png)
   
#### 3. create routes
   #### inside routes, create todo.model.js
   ![Image](https://github.com/miaypc/Notes/blob/master/images/backend-7.png)
   
   ![Image](https://github.com/miaypc/Notes/blob/master/images/backend-12.png)
   
#### 4. Check in Postman
   ![Image](https://github.com/miaypc/Notes/blob/master/images/backend-13.png)

## Read-Get

#### 1. in todo.services.js (remember to export)
![Image](https://github.com/miaypc/Notes/blob/master/images/backend-14.png)

#### 2. in todo.controllers.js (remember to export)
![Image](https://github.com/miaypc/Notes/blob/master/images/backend-15.png)

#### 3. in todo.routers.js
![Image](https://github.com/miaypc/Notes/blob/master/images/backend-16.png)

#### 3. in Postman
![Image](https://github.com/miaypc/Notes/blob/master/images/backend-17.png)

## getById,Patch-Update,Delete
   #### follow the same steps as before.
   
 
#### 1. in todo.services.js (remember to export)
![Image](https://github.com/miaypc/Notes/blob/master/images/backend-18.png)

#### 2. in todo.controllers.js (remember to export)
![Image](https://github.com/miaypc/Notes/blob/master/images/backend-19.png)

#### 3. in todo.routers.js
![Image](https://github.com/miaypc/Notes/blob/master/images/backend-20.png)


# Front

## create create app

#### outside Back folder, in terminal: npx creat-react-Front

### review Hooks

function App(){
	const [counter, setCounter] = React.useState(0);
	return
		<div>
			<h1>{counter}</h1>
			<button onClick ={() => setCounter(counter + 1 )}> increment </button>
		</div>
}


### review Reducer
#### if we want to have mutiple actions, we can create reducer.

function reducer(state, action) {
swict
function App(){
   const initialState = {
   counter: 0
   }
   const [counter, setCounter] = React.useState(0);
   const [state, dispatch] = React. useReducer(reducer, initialState)
   return
      <div>
         <h1>{counter}</h1>
         <button onClick ={() => setCounter(counter + 1 )}> increment </button>
      </div>
}
