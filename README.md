# Movie Explorer

Movie Explorer is a React + Vite web app for browsing movies, searching titles, and managing a favorites list.

## Features

- Search and browse movie content from the home page.
- Add movies to a favorites list.
- Remove movies from favorites.
- Favorites are persisted in `localStorage` so they remain after page refresh.
- Client-side routing for Home, Favorites, Login, and Signup pages.
- Global state management with Redux Toolkit.

## Tech Stack

- React 19
- Vite 7
- React Router
- Redux Toolkit + React Redux
- Tailwind CSS 4

## Project Structure

```text
src/
  component/
    Header.jsx
    Moviecard.jsx
    SearchBar.jsx
    Favmovie.jsx
    Login.jsx
    Signup.jsx
  redux/
    CreateSlice.js
    store.js
  App.jsx
  Layout.jsx
  main.jsx
```

## Getting Started

### 1) Prerequisites

- Node.js 18+ (recommended: latest LTS)
- npm

### 2) Install dependencies

```bash
npm install
```

### 3) Run development server

```bash
npm run dev
```

Then open the local URL shown in your terminal (typically `http://localhost:5173`).

## Available Scripts

- `npm run dev` — start development server
- `npm run build` — create production build
- `npm run preview` — preview production build locally
- `npm run lint` — run ESLint

## Favorites Persistence

Favorites are saved in browser `localStorage` under the key:

- `favmovie`

This is handled in the Redux slice (`src/redux/CreateSlice.js`) when adding/removing items.

## Notes

- This project currently focuses on front-end behavior and local persistence.
- If you plan to connect a real movie API, add your API integration inside the search/listing components and keep secret keys in environment variables.
