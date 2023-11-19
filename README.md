<div>
  <h1>⚡️Todo App</h1>
</div>


## Introduction

A To-Do list application developed using React and Typescript. It enables users to seamlessly add, delete and mark tasks as completed.

## Technologies used

This project follows a custom structure that combines the following:

- [`TypeScript`](https://www.typescriptlang.org/) for extending JavaScript to be typed.
- [`React`](https://reactjs.org/) as the view layer of the app;
- [`Redux-Toolkit`](https://redux-toolkit.js.org/) for managing the app's state;
- [`Antd`](https://ant.design/) as the UI library;
- [`Webpack`](https://webpack.js.org/) as the main build tool for this app;

... and some [more stuff](./package.json).


## Challenges I face and how I approached them

### Description

Initially, task deletion funcionality had a delay in updating the UI, causing an inconsistent user experience.

### Approach/Analysis

Invesigating the issue, I found that the Redux store update for the task deletion was asynchroneous, leading to a brief delay in reflecting the change in the UI.

### Solution

To address the issue, I optimized the Redux action for task deletion to dispatch a loading state immediately. I then utilized async/await within the Redux thunk to ensure synchronous execution, resulting in a smoother and more responsive UI update when deleting tasks.


### Setting up the project

Clone the repository and run the following:

    $ npm install

### Running the dev server

Running the following will start the dev server and will automatically open the webapp in your
default browser:

    $ npm start

### Building

In order to build the app for production, run the build script:

    $ npm run build


## Project structure

Everything goes under the `./src` folder.


---

