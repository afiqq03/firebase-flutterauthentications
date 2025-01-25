# Firebase Authentication App

A basic Flutter application demonstrating Firebase Authentication implementation. You can design your own ui. This is just a basic flutter connected with firebase

## Features

- Email/Password Authentication
- Login/Register functionality
- Error handling
- Protected routes
- Persistent authentication state

## Setup Instructions

1. Clone the repository
git clone <repository-url>
cd your_app_name

2. Install dependencies
flutter pub get

3. Configure Firebase
Create a new Firebase project at Firebase Console
Enable Email/Password authentication
Download google-services.json (Android) and GoogleService-Info.plist (iOS)
Place configuration files in respective directories
Run flutterfire configure

4. Run the app
flutter run

5. Project structure should be like this
lib/
├── screens/
│   ├── login.dart         # Login screen
│   ├── register.dart      # Registration screen
│   └── homescreen.dart    # Home screen (protected)
├── firebase_options.dart  # Firebase configuration
└── main.dart             # App entry point

6. App flows
- user open app 
App checks authentication state
Redirects to Login/Register if not authenticated
Shows Home screen if authenticated

- Login process
User enters email/password
Validates input
Shows error messages if invalid
Redirects to Home screen on success

- Registration Process
User enters email/password
Validates input
Creates new account
Automatically logs in
Redirects to Home screen

7. License
This project is licensed under the MIT License - see the LICENSE file for details
