# AmbAnime

An anime browsing web app built with **React (Create React App)** + **Firebase**.

Data is fetched from the **Jikan API** (MyAnimeList unofficial API): https://api.jikan.moe/v4 (see `src/services/api.js`).

## Features
- Browse & search anime
- Anime detail pages (characters, recommendations)
- User authentication (Firebase Auth)
- User data in Firestore (favorites, watchlist)
- Reviews stored in Firestore
- Basic admin utilities (e.g. list users / delete user data)

## Tech stack
- React (CRA)
- Firebase (Auth + Firestore)
- React Router
- Framer Motion
- Recharts

## Run locally
```bash
npm install
npm start
```

## Notes
- The Jikan API is rate-limited; this project includes simple retry/backoff handling.
- Firebase config is currently in `src/services/firebase.js`.

## Portfolio notes
- Integrating a public API + handling rate limits
- Full auth + user state with Firebase
- CRUD features (favorites/watchlist/reviews)
