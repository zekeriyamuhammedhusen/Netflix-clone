# Netflix Clone

A React-based Netflix UI clone that fetches movie and TV data from TMDB and plays trailers directly in the page.

## Live Demo

https://zekeriyamuhammedhusen.github.io/Netflix-clone

## Features

- Netflix-style homepage layout with reusable sections
- Dynamic hero banner with a random Netflix Original
- Multiple content rows (Trending, Top Rated, Action, Comedy, Horror, Romance, Documentaries, TV Shows)
- Trailer playback using YouTube embeds
- Responsive poster rows with large and standard card styles
- Header and footer inspired by Netflix navigation

## Tech Stack

- React (Create React App)
- Axios (API requests)
- TMDB API (movie and TV metadata)
- movie-trailer + react-youtube (trailer lookup and playback)
- Material UI Icons
- GitHub Pages (deployment)

## Project Structure

```text
src/
	Components/
		Banner/
		Footer/
		Header/
		Row/
		RowList/
	pages/
		Home/
	utils/
		axios.js
		requests.js
```

## Getting Started

### 1. Clone the repository

```bash
git clone <your-repository-url>
cd netflix-clone
```

### 2. Install dependencies

```bash
npm install
```

### 3. Configure environment variables

Create a `.env` file in the project root:

```env
REACT_APP_API_KEY=your_tmdb_api_key_here
```

Get your API key from TMDB: https://www.themoviedb.org/settings/api

### 4. Start the development server

```bash
npm start
```

App will run at: http://localhost:3000

## Available Scripts

### `npm start`

Runs the app in development mode.

### `npm test`

Launches the test runner.

### `npm run build`

Builds the app for production into the `build/` directory.

### `npm run deploy`

Builds and deploys the app to GitHub Pages using the `homepage` field in `package.json`.

## Deployment Notes

- Ensure the `homepage` value in `package.json` matches your GitHub Pages URL.
- Run:

```bash
npm run deploy
```

## API Endpoints Used (TMDB)

- Trending
- Netflix Originals
- Top Rated
- Action
- Comedy
- Horror
- Romance
- Documentaries
- TV Popular

All endpoint paths are configured in `src/utils/requests.js`.

## Security Note

- Do not commit real API keys to version control.
- If an API key was exposed, regenerate it from your TMDB account and update `.env`.

## Acknowledgements

- Netflix (UI inspiration)
- TMDB for the movie/TV data API

This product uses the TMDB API but is not endorsed or certified by TMDB.
