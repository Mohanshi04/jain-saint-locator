# Jain Saint Locator

A React Native (Expo) mobile application that helps devotees track publicly available vihar routes, saint movements, and event information in a structured, community-driven, and privacy-respecting manner.

---

## Features

- Phone number–based authentication using Firebase Auth.
- User roles: Viewer, Signed-In Viewer, Volunteer.
- Saint profiles with English/Hindi names, sect, gender, guru details, diksha date, group info.
- Event management supporting multiple event types (Pravachan, Diksha, Pratishtha, Vihar, Meetings).
- Map view with pins, user location, and nearby saint calculation (Haversine).
- Real-time updates powered by Cloud Firestore.
- Volunteer capabilities to add or update saint information, events, and photos (with verification planned).
- Search and filtering across saints and events.
- List view and map view for better accessibility.

---

## Tech Stack

- Framework: React Native (Expo)
- Language: TypeScript / JavaScript
- Backend: Firebase (Firestore, Authentication, Storage, Cloud Functions)
- Maps: react-native-maps (Google Maps Provider)
- Location: Expo Location
- UI Components: React Native core components, Expo Vector Icons

---

## Installation

1. Clone the repository  
   git clone https://github.com/Mohanshi04/jain-saint-locator.git  
   cd jain-saint-locator

2. Install dependencies  
   npm install

3. Setup Firebase  
   - Create a Firebase project
   - Add your Firebase config inside config/firebase.ts

4. Start the application  
   npx expo start  
   Then open it using Expo Go or an emulator.

---

## Environment Notes

- Firebase Phone Auth requires SHA-1 and SHA-256 keys for Android.
- Ensure Google Maps API key is configured for react-native-maps.
- Cloud Functions optional but recommended for background tasks.

---

## Screens Overview

- Home: Saint list, search, and details.
- Map: Pins for saints, user location, nearby calculation.
- Events: List of upcoming events with filters.
- Event Detail: Host saint, time, description, and poster.
- Profile: Settings, volunteer signup, and user details.

---

## Security

- Firestore rules restrict sensitive writes to approved volunteers only.
- Coordinates and sensitive data are posted only when permitted.
- Strict access control based on user roles.

---

## Repository

https://github.com/Mohanshi04/jain-saint-locator
