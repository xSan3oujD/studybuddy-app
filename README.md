# StudyBuddy + Firebase (Google sign-in and sync)

1. console.firebase.google.com > Add project (free Spark plan, no card needed).
2. Build > Authentication > Get started > Sign-in method > enable Google.
3. Build > Firestore Database > Create database (production mode), then open Rules and paste firestore.rules > Publish.
4. Project settings > Your apps > add a Web app (</>). Copy the config into firebase-config.js.
5. Host it (recommended, free): install Node, then run
     npm i -g firebase-tools
     firebase login
     firebase init hosting   (public folder: . ; single-page app: No; do not overwrite files)
     firebase deploy
   Your app is live at https://YOUR_PROJECT.web.app and installable on phones.
6. Authentication > Settings > Authorized domains: add any other domain you host on (Netlify, GitHub Pages...).
