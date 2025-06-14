# Notes for Developing a Front-End Project
[Back](../README.md)

## Overview
Notes for developing a front-end project using React Framework.

## Technology Stacks
Tech | Purpose | Link
---- | ---- | ----
Redux | State management | [E-link](https://redux-toolkit.js.org/introduction/getting-started)
Redux Thunk | Define data fetching | [E-link](https://redux.js.org/usage/writing-logic-thunks)
React Framework | Frontend framework | None
Axios Package | Handle http requests | [E-Link](https://axios-http.com/docs/intro)
Selectors | Abstract of the structure of the state | [E-link](https://redux.js.org/usage/deriving-data-selectors)
React router | Manage route | [E-link](https://reactrouter.com/start/data/installation)


## Steps to create a React Frontend project
1. `npm create vite@latest`
2. `npm install`
3. `npm run dev`

## Steps to create a Backend for Frontend project
1. Create a folder
2. cd to the new folder
3. `npm init -y`
4. `npm install express` to install express package
5. Create `src` folder
6. Create file `server.js`

## Add redux to project
- Redux Toolkit: `npm install @reduxjs/toolkit`
- React bindings: `npm install react-redux`
- Redux Thunk: already in the `@reduxjs/toolkit` package
- Selector
    - `useSelector` in the `react-redux` package
    - `createSelector` in the `@reduxjs/toolkit` package

## Add Axios to project
- `npm install axios`

## Add React router to project
- `npm i react-router`
