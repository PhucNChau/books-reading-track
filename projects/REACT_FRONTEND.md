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

## Steps to work with a new react project
1. Create folder structure
    <details>

    <summary>Example</summary>
    ```
    my-vite-app/
    ├── public/
    │   └── favicon.svg
    ├── src/
    │   ├── assets/
    │   │   ├── images/
    │   │   └── styles/
    │   │       └── global.css
    │   ├── components/
    │   │   ├── ui/                  # Reusable common UI components
    │   │   │   ├── Button.tsx
    │   │   │   └── Card.tsx
    │   │   ├── layout/              # Site layout parts
    │   │   │   ├── Header.tsx
    │   │   │   └── Footer.tsx
    │   │   └── detail/              # Detail-page-specific components
    │   │       ├── DetailHeader.tsx
    │   │       ├── InfoSection.tsx
    │   │       └── RelatedItems.tsx
    │   ├── pages/
    │   │   ├── Home.tsx
    │   │   ├── About.tsx
    |   │   ├── Dashboard/
    |   │   │   ├── DashboardLayout.tsx    # Shared layout for all dashboard routes
    |   │   │   ├── Overview.tsx           # /dashboard/overview
    |   │   │   ├── Settings.tsx           # /dashboard/settings
    |   │   │   └── index.tsx              # /dashboard (default landing)
    │   │   └── DetailPage.tsx       # Handles dynamic loading based on route param
    │   ├── routes/
    │   │   └── AppRoutes.tsx        # Central place for React Router DOM routes
    │   ├── services/
    │   │   └── api.ts               # Axios or fetch logic
    │   ├── types/
    │   │   └── item.ts              # Custom interfaces/types
    │   ├── utils/
    │   │   ├── formatDate.ts
    │   │   └── constants.ts
    |   ├── store/                       # Central Redux setup
    │   |   ├── index.ts                 # Root store configuration
    │   |   └── rootReducer.ts          # Combine reducers here
    |   ├── features/
    |   │   ├── items/                  # A feature (e.g. items, products, users)
    |   │   │   ├── itemsSlice.ts       # Redux slice (reducers + actions)
    |   │   │   ├── itemsActions.ts     # Thunk async actions
    |   │   │   ├── itemsSelectors.ts   # Selectors for this feature
    |   │   │   └── itemsTypes.ts       # Types/interfaces (optional)
    |   │   └── user/                   # Another feature
    |   │       ├── userSlice.ts
    |   │       ├── userActions.ts
    |   │       ├── userSelectors.ts
    |   │       └── userTypes.ts
    │   ├── App.tsx
    │   ├── main.tsx                 # Entry point for Vite
    │   └── config/
    │       └── env.ts               # Environment variables and config helpers
    ├── .env                         # Environment variables
    ├── vite.config.ts
    ├── tsconfig.json
    ├── package.json
    └── README.md
    ```
    </details>

2. Add `react-router` package, create page components and app routes

3. 