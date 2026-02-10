# Movie Explorer

Movie Explorer is a React + Vite web app that lets users search movies through The Movie Database (TMDB) API and save favorites using Redux with `localStorage` persistence.

## Features

- Search movies from TMDB in real time.
- Browse results with posters, titles, and release dates.
- Add movies to a favorites list.
- Remove movies from favorites.
- Favorites persist in the browser via `localStorage`.
- Client-side navigation with React Router.

## Tech Stack

- React 19
- Vite 7
- Redux Toolkit + React Redux
- React Router DOM
- Tailwind CSS

## Project Structure

```text
src/
  component/
    Header.jsx
    SearchBar.jsx
    Moviecard.jsx
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

### Prerequisites

- Node.js 18+ (recommended)
- npm

### Installation

```bash
npm install
```

### Run in Development

```bash
npm run dev
```

Then open the local URL shown by Vite (typically `http://localhost:5173`).

### Build for Production

```bash
npm run build
```

### Preview Production Build

```bash
npm run preview
```

## Available Routes

- `/` — Home/Search page
- `/favmovie` — Favorite movies
- `/login` — Login page
- `/Signup` — Signup page

## Notes

- The app currently calls TMDB directly from the frontend using an API key in source.
- For production apps, move secrets to environment variables and call APIs through a backend.

## License

This project is currently unlicensed.
