# Task Manager — Frontend

React single-page app for the Task Manager.

Backend: [task-manager-backend](https://github.com/IevaGurencik/task-manager-backend)

## Tech stack

- React 19, React Router 7
- Axios
- Bootstrap 5, CSS Modules
- Create React App

## Features

- Login page and protected routes
- Task list with creating tasks in a modal and deleting them
- Attaching files to tasks, downloading and deleting attachments
- Backend URL configured through an environment variable

<!-- Add a screenshot of the main page here:
![Task list](docs/screenshot.png)
-->

## Getting started

**Requirements:** Node.js 18+, running [backend](https://github.com/IevaGurencik/task-manager-backend)

1. Install dependencies:
   ```bash
   npm install
   ```
2. Create a `.env` file in the project root with the backend URL:
   ```
   REACT_APP_HTTP_PROXY=http://localhost:8080
   ```
3. Start the dev server:
   ```bash
   npm start
   ```
   The app opens at http://localhost:3000.

## Build

```bash
npm run build
```

The production build is created in the `build/` folder.

## Project structure

```
src
├── client/       # Axios instance and API base URL
├── components/   # UI components, auth context, modals, layout
├── routes/       # Pages, root layout, protected route
└── index.js      # Router setup
```
