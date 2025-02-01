# To-Do List Application

This is a simple To-Do List application built using React. The application allows users to add, mark as complete, and delete to-do items. It also keeps track of the total and completed tasks.

## Application Structure

The project has the following structure:

project-root/
│
├── public/
│ ├── index.html
│ └── ...
│
├── src/
│ ├── App.js
│ ├── App.css
│ ├── App.test.js
│ ├── components/
│ │ ├── ToDoForm.js
│ │ ├── ToDoForm.test.js
│ │ ├── ToDoItem.js
│ │ ├── ToDoItem.test.js
│ │ ├── ToDoList.js
│ │ └── ToDoList.test.js
│ └── index.js
│
├── package.json
└── README.md


### Components

- **App.js**: The main component that manages the state and renders the `ToDoForm` and `ToDoList` components.
- **ToDoForm.js**: A form component that allows users to add new to-do items.
- **ToDoItem.js**: A component that renders an individual to-do item with options to mark it as complete or delete it.
- **ToDoList.js**: A component that renders a list of `ToDoItem` components.

### Tests

- **App.test.js**: Tests for the `App` component to ensure correct rendering and functionality.
- **ToDoForm.test.js**: Tests for the `ToDoForm` component to ensure correct rendering and functionality.
- **ToDoItem.test.js**: Tests for the `ToDoItem` component to ensure correct rendering and functionality.
- **ToDoList.test.js**: Tests for the `ToDoList` component to ensure correct rendering and functionality.

## How to Run the Application

### Prerequisites

- Node.js (v14 or higher recommended)
- npm (v6 or higher) or yarn (v1.22 or higher)

### Steps

1. Clone the repository:

git clone https://github.com/chessmanpk/React-Assignment-ToDo


Install the dependencies:
npm install

Run the application:
npm start

This will start the development server and open the application in your default web browser. The application should be running on http://localhost:3000.

To run the tests, use the following command:
npm test

This will run all the test files using Jest and React Testing Library.



Challenges Faced and Solutions

1. Handling Component State
Managing the state of multiple components and ensuring they update correctly in response to user actions was a bit challenging. This was resolved by using React's state hooks (useState) and effect hooks (useEffect) to manage and synchronize state between components.

2. Local Storage Integration
Persisting the to-do list in the browser's local storage required careful handling to ensure data consistency. The solution was to use useEffect to save the to-do list to local storage whenever it changed, and to initialize the state from local storage when the application loads.

3. Writing Tests
Writing tests for the components to cover various scenarios was a learning curve, especially for simulating user interactions with fireEvent. By leveraging Jest and React Testing Library, comprehensive tests were written to ensure the components render correctly and handle user actions as expected.

....
