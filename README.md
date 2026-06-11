# Secure Web Browser Application

A modern Android web browser application developed using Kotlin and Jetpack Compose. The application provides secure Google authentication, in-app web browsing, local browsing history management, and notification support while following modern Android development practices.

## Features

### Authentication

* Google Sign-In using Firebase Authentication
* Secure user session management
* Automatic login persistence
* Logout functionality

### Home Screen

* URL input field
* Open website functionality
* Image carousel with page indicators
* Navigation to browsing history
* User session controls

### Web Browsing

* WebView-based website rendering
* Loading progress indicator
* Error handling for network failures
* Current URL tracking
* Back and close navigation controls
* State restoration during configuration changes

### History Management

* Local browsing history storage using Room Database
* Visit count tracking
* Last visited timestamp tracking
* Clear history functionality

## Technologies Used

* Kotlin
* Jetpack Compose
* Firebase Authentication
* Google Sign-In
* Room Database
* MVVM Architecture
* ViewModel
* Kotlin Coroutines
* WebView
* Material Design 3

## Architecture

The application follows the MVVM (Model-View-ViewModel) architecture pattern.

### Components

* UI Layer (Jetpack Compose)
* ViewModel Layer
* Repository Layer
* Room Database Layer
* Firebase Authentication Layer

## Database Schema

### History Table

| Field           | Type   | Description          |
| --------------- | ------ | -------------------- |
| id              | Int    | Primary Key          |
| url             | String | Website URL          |
| title           | String | Website Title        |
| visitCount      | Int    | Number of Visits     |
| lastVisitedTime | Long   | Last Visit Timestamp |

## Project Structure

```text
app/
├── data/
│   ├── database/
│   ├── repository/
│   └── model/
├── ui/
│   ├── screens/
│   ├── components/
│   └── navigation/
├── viewmodel/
├── notification/
└── auth/
```

## Setup Instructions

### Clone Repository

```bash
git clone https://github.com/yourusername/Secure-Web-Browser-App.git
```

### Open Project

1. Open Android Studio
2. Select Open Project
3. Sync Gradle files

### Firebase Setup

1. Create a Firebase Project
2. Enable Authentication
3. Enable Google Sign-In
4. Download google-services.json
5. Place it inside the app directory

### Run Application

```bash
./gradlew assembleDebug
```

or run directly from Android Studio.

## Challenges Faced

* Managing WebView lifecycle correctly
* Handling configuration changes
* Implementing history tracking without duplicate entries
* Managing Firebase authentication sessions
* Supporting multiple Android versions for notifications

## Future Improvements

* Browser bookmarks
* Download manager
* Multiple tabs support
* Dark mode customization
* Browser search suggestions
* Website favorites
* Browser cache management

## Author

Mohit Kumawat

Android Developer | Kotlin | Firebase | Jetpack Compose
