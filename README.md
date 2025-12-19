# react-native-firebase

2️⃣ React Native + Firebase Backend Commands
# Firebase install
npm install firebase

# Firebase config file create
touch firebaseConfig.js

// firebaseConfig.js
import { initializeApp } from 'firebase/app';
import { getAuth } from 'firebase/auth';
import { getFirestore } from 'firebase/firestore';

const firebaseConfig = {
  apiKey: "YOUR_API_KEY",
  authDomain: "YOUR_AUTH_DOMAIN",
  projectId: "YOUR_PROJECT_ID",
  storageBucket: "YOUR_STORAGE_BUCKET",
  messagingSenderId: "YOUR_SENDER_ID",
  appId: "YOUR_APP_ID"
};

const app = initializeApp(firebaseConfig);
export const auth = getAuth(app);
export const db = getFirestore(app);


Commands for Firebase deployment:

# Optional: Firebase Functions
npm install -g firebase-tools
firebase login
firebase init
firebase deploy
Link: Firebase + React Native Guide
