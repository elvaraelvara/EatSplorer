
# Eatsplorer! - Food Discovery App for Culinary SMEs

## 📌 Description
**Eatsplorer!** is a mobile-based food discovery application designed to enhance the exposure and revenue of small-scale culinary SMEs in Indonesia. By utilizing GPS and camera features, the app allows users to find nearby dining spots, leave reviews, and save favorite places. Eatsplorer! aims to help small culinary businesses reach more customers with minimal investment while offering a personalized and seamless food discovery experience for users.

---

## 🎯 Features

### 1️⃣ **Location Feature**
- Real-time user location detection using **Expo Location**.
- Display user location on a map with **react-native-maps**.
- Provide a list of nearby culinary SMEs based on user location.

### 2️⃣ **Review Feature**
- Users can leave reviews and upload photos of dining places.
- Allow image uploads from gallery or directly from the camera.
- Display a list of reviews from other users.

### 3️⃣ **Search Feature**
- Users can search for dining places by name.
- Real-time search with Firebase Realtime Database.

### 4️⃣ **Bookmark Feature**
- Users can save their favorite dining spots for future visits.

### 5️⃣ **Authentication Feature**
- User registration and login with **Firebase Authentication**.
- Only registered users can submit reviews.

### 6️⃣ **Additional Features**
- **Sort by rating**: Display top-rated restaurants.
- **Restaurant categories**: Filter by cuisine type (Indonesian, Japanese, Western, etc.).

---

## 🛠️ Technologies Used

### 📌 **Frontend**
- **React Native** → Primary framework for mobile development.
- **Expo** → Simplifies development and testing.
- **NativeWind** → Tailwind CSS-based styling for React Native.
- **OpenStreetMap API** → Displays maps and restaurant locations.
- **Expo Location** → Retrieves real-time user location.
- **React Native Maps** → Displays maps and user location markers.

### 🔥 **Backend & Database**
- **Firebase Authentication** → Manages user registration and login.
- **Firebase Realtime Database** → Stores restaurant, user, and review data.
- **Firebase Storage** → Manages and stores user-uploaded images.

---

## 🚀 Installation & Setup

### 1️⃣ **Clone the Repository**
```sh
git clone https://github.com/username/eatsplorer.git
cd eatsplorer
```

### 2️⃣ **Install Dependencies**
```sh
npm install
```

### 3️⃣ **Run the App with Expo**
```sh
npx expo start
```

### 4️⃣ **Run on Emulator or Physical Device**
- Scan the displayed QR Code using **Expo Go** on an Android/iOS device.
- If using an emulator, ensure Android Emulator or iOS Simulator is installed.

---

## ⚙️ Firebase Configuration

1. Create a Firebase account and project at [Firebase Console](https://console.firebase.google.com/).
2. Enable **Authentication**, **Realtime Database**, and **Storage**.
3. Download the `google-services.json` (for Android) or `GoogleService-Info.plist` (for iOS) file and place it in the appropriate directory.
4. Configure Firebase in the project:
   ```js
   import { initializeApp } from 'firebase/app';
   import { getAuth } from 'firebase/auth';
   import { getDatabase } from 'firebase/database';
   import { getStorage } from 'firebase/storage';

   const firebaseConfig = {
     apiKey: 'YOUR_API_KEY',
     authDomain: 'YOUR_AUTH_DOMAIN',
     databaseURL: 'YOUR_DATABASE_URL',
     projectId: 'YOUR_PROJECT_ID',
     storageBucket: 'YOUR_STORAGE_BUCKET',
     messagingSenderId: 'YOUR_MESSAGING_SENDER_ID',
     appId: 'YOUR_APP_ID',
   };

   const app = initializeApp(firebaseConfig);
   export const auth = getAuth(app);
   export const database = getDatabase(app);
   export const storage = getStorage(app);
   ```

---

## 📌 Folder Structure
```
📂 eatsplorer
│── 📂 assets       # Stores images and icons
│── 📂 components   # Reusable UI components
│── 📂 screens      # Main app screens
│── 📂 functions    # Core application functions
│── App.js         # Main application entry point
│── firebase.js    # Firebase configuration
│── package.json   # Project dependencies
│── README.md      # Project documentation
```

---

## 📌 Development Roadmap
- [x] Implement real-time location detection
- [x] Integrate Firebase for authentication and database
- [x] Enable review submissions with images
- [x] Add restaurant sorting by rating and categories
- [ ] Implement online payment for SMEs
- [ ] Develop AI-based recommendation feature


## 📄 Documentation  

You can access the full documentation [here](https://docs.google.com/document/d/1-1hM5sfAQO6UU-FmhlV7bBjy6ntUQuxwMxL_tZV1NRk/edit?usp=sharing).  
