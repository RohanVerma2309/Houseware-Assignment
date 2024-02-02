# Getting Started with Create React App

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in your browser.

The page will reload when you make changes.\
You may also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.\
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.\
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `npm run eject`

**Note: this is a one-way operation. Once you `eject`, you can't go back!**

If you aren't satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you're on your own.

You don't have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn't feel obligated to use this feature. However we understand that this tool wouldn't be useful if you couldn't customize it when you are ready for it.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).
   
### Code Splitting

This section has moved here: [https://facebook.github.io/create-react-app/docs/code-splitting](https://facebook.github.io/create-react-app/docs/code-splitting)

### Analyzing the Bundle Size

This section has moved here: [https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size](https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size)

### Making a Progressive Web App

This section has moved here: [https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app](https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app)

### Advanced Configuration

This section has moved here: [https://facebook.github.io/create-react-app/docs/advanced-configuration](https://facebook.github.io/create-react-app/docs/advanced-configuration)

### Deployment

This section has moved here: [https://facebook.github.io/create-react-app/docs/deployment](https://facebook.github.io/create-react-app/docs/deployment)

### `npm run build` fails to minify

This section has moved here: [https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify](https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify)

# Todo List App Test Plan

## Introduction
This document outlines the testing strategy for the Todo List React app. The goal is to ensure the reliability and functionality of each component and feature within the application.

## Testing Tools
- Jest: A JavaScript testing framework.
- React Testing Library: A testing utility for React.

## Folder Structure



## Test Cases

### TodoItem Component
#### Test Type: Unit Testing

1. **Rendering TodoItem**
   - **Case:** Renders without crashing.
   - **Case:** Renders the correct task text.
   - **Case:** Renders the correct completion status.

2. **Toggle TodoItem Completion**
   - **Case:** Clicking on the TodoItem toggles completion status.
   - **Case:** Completed TodoItem has appropriate styling.

3. **Delete TodoItem**
   - **Case:** Clicking on the delete button removes the TodoItem.
   - **Case:** Confirming deletion removes the TodoItem.

4. **Update TodoItem Text**
   - **Case:** Double-clicking on the text allows editing.
   - **Case:** Editing the text updates the TodoItem.

5. **Render Different TodoItem Variations**
   - **Case:** Renders TodoItem with different text.
   - **Case:** Renders incomplete TodoItem without "completed" class.

### TodoList Component
#### Test Type: Integration Testing

1. **Rendering TodoList**
   - **Case:** Renders without crashing.
   - **Case:** Renders the correct number of TodoItems.

2. **Adding TodoItems**
   - **Case:** Adding a new task updates the TodoList.
   - **Case:** Adding multiple tasks updates the TodoList accordingly.

3. **Filtering TodoItems**
   - **Case:** Clicking on "All" shows all TodoItems.
   - **Case:** Clicking on "Active" shows only active TodoItems.
   - **Case:** Clicking on "Completed" shows only completed TodoItems.

4. **Marking TodoItems as Completed**
   - **Case:** Clicking on a TodoItem marks it as completed.
   - **Case:** Completed TodoItems have appropriate styling.

5. **Clearing Completed TodoItems**
   - **Case:** Clicking "Clear Completed" removes completed TodoItems.
   - **Case:** Clearing does not affect active TodoItems.

6. **Rendering an Empty TodoList**
   - **Case:** Renders a message when there are no tasks.
   - **Case:** No message is displayed when there are tasks.

7. **Marking TodoItems as Uncompleted**
   - **Case:** Clicking on a completed TodoItem marks it as uncompleted.

8. **Editing TodoItem Text**
   - **Case:** Double-clicking on the text of a TodoItem allows editing.
   - **Case:** Editing the text updates the TodoItem.

## Running Tests
1. Install dependencies: `npm install`
2. Run tests: `npm test`

