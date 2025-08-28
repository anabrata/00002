# Shortly — URL Shortener (Netlify Functions + Firebase)

This project is a ready-to-deploy URL shortener using a React frontend, Netlify Functions, and Firestore (Firebase) for storage.

## Quick setup
1. Create a Firebase project and enable Firestore (Native mode). Create a Web app and copy the Firebase config values.
2. On Netlify: create a new site from the repository, set environment variables (see `.env.example`) in Netlify site settings, and deploy.
3. Ensure Netlify builds the project (the repo uses Parcel in this scaffold). Functions will be detected from `netlify/functions`.
4. Optional: set a custom domain in Netlify for better indexing & brandable short links.

## Files included
- package.json
- netlify.toml
- .env.example
- public/_redirects
- src/index.html, src/index.jsx, src/App.jsx
- netlify/functions/create.js, netlify/functions/redirect.js

## Notes
- Replace the `.env` values in Netlify with your Firebase config.
- For production security use Firebase Admin SDK with service account in functions.
- Add Firestore rules to prevent abuse.
