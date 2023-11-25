
# React Todo App


This simple React Todo App is designed to help you manage your tasks effectively. It utilizes the Context API for state management and localStorage for persistent data storage. Whether you want to add, update, or delete tasks, this app has got you covered.
https://anafariya.github.io/reactTodo/

![Screenshot (45)](https://github.com/anafariya/reactTodo/assets/70438803/21ee0f59-f574-4617-808f-da20e8b6b0c0)

# Features

* *Add Todo*: Easily add new tasks with a title and description.
* *Update Todo*: Modify existing tasks to keep your information up-to-date.
* *Delete Todo*: Remove tasks that are no longer relevant or completed.
* *Toggle Complete*: Mark tasks as complete or incomplete with a simple click.
* *Persistent Storage*: Your todos are stored in the browser's localStorage, ensuring that your tasks are preserved even if you close or refresh the page.


# Technologies Used
* *React*: A JavaScript library for building user interfaces.
* *Context API*: Used for state management, providing a way to pass data through the component tree without having to pass props down manually.
* *localStorage*: Utilized to store and retrieve todos locally in the user's browser.

 # Getting Started
**Clone the repository**:

*Copy code*
```
git clone 
https://github.com/anafariya/react-todo-app.git
```
*Install dependencies:* 
```
Copy code
cd react-todo-app
npm install
```
*Start the development server:*
```bash
Copy code
npm start
```

# How to Use
* *Add Todo*: Enter a title and description in the form and click the "Add Todo" button.

* *Update Todo*: Click on a todo to open the update form. Make your changes and click "Save Changes."

* *Delete Todo*: Click on the delete icon next to a todo to remove it from the list.

* *Toggle Complete*: Click on a todo to mark it as complete or incomplete.

  # Local Storage for Persistent Data
Todos are stored in the browser's localStorage, allowing users to access their tasks even after closing or refreshing the page.

javascript
```
Copy code
// src/components/App.js
useEffect(() => {
  const todos = JSON.parse(localStorage.getItem('todos'));

  if (todos && todos.length > 0) {
    setTodos(todos);
  }
}, []);

useEffect(() => {
  localStorage.setItem('todos', JSON.stringify(todos));
}, [todos]);
```
Feel free to explore the code and make it your own! Happy task managing!

