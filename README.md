# Task Manager App

## App Description
A simple Android application for managing personal tasks and notes. Users can create, view, complete, and delete tasks. All data is stored locally on the device.

## Features
- Add new tasks with title and description
- View all tasks in a clean list
- Mark tasks as completed
- Delete tasks
- Data persists after app restart
- Handles screen rotation properly

## Screenshots
*(Take screenshots from your emulator/phone and add them here)*

1. Main Screen with Task List
2. Add Task Screen

## Design Choices Explained

### 1. Architecture: MVVM (Model-View-ViewModel)
- **Why**: Separates concerns and makes code more maintainable
- **Benefit**: UI code is separate from business logic and data handling

### 2. Data Storage: Room Database
- **Why**: More robust than SharedPreferences for structured data
- **Benefit**: Automatic background threading, LiveData observation, type safety

### 3. UI Design: Material Design Guidelines
- **Why**: Consistent with Android standards
- **Benefit**: Familiar user experience, accessibility compliance

### 4. Secure Coding Practices Implemented:
1. **Input Validation**: All user inputs are validated before processing
2. **Safe Data Storage**: Sensitive data is not hard-coded, database is properly encrypted by Room
3. **State Preservation**: UI state is preserved during configuration changes

## How to Build and Run
1. Open project in Android Studio
2. Sync Gradle files
3. Run on emulator or physical device (API 26+)

## Technologies Used
- Kotlin
- Android Jetpack Components (Room, ViewModel, LiveData)
- Material Design Components
- Coroutines for background operations
