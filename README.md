# Teacher Diary

An Android app for teachers to manage student records and daily tasks. Students are stored locally using SQLite, with a simple UI to add, list, search, and view student information.

## Features

- Add students via a form (`AddForm`)
- Browse all students in a list (`AllStudents`)
- View individual student details (`StudentInfo`)
- Search students and manage tasks
- Local persistence with SQLite (`DBHelper`)

## Tech Stack

- **Language:** Java
- **Build:** Gradle
- **Min SDK:** 27 · **Target/Compile SDK:** 33
- **Libraries:** AndroidX AppCompat, Material Components, ConstraintLayout
- **Package:** `com.bilal.teacherdiary`

## Getting Started

### Prerequisites

- Android Studio (Giraffe or newer recommended)
- JDK 8+
- Android SDK 33

### Build & Run

```bash
# Clone the repository
git clone <repo-url>
cd diary

# Build a debug APK
./gradlew assembleDebug

# Install on a connected device/emulator
./gradlew installDebug
```

Or open the project in Android Studio and press **Run**.

### Tests

```bash
./gradlew test              # unit tests
./gradlew connectedAndroidTest   # instrumented tests (device/emulator required)
```

## Project Structure

```
app/src/main/java/com/bilal/teacherdiary/
├── MainActivity.java     # entry screen
├── AddForm.java          # add a student
├── AllStudents.java      # list of students
├── StudentInfo.java      # student detail view
├── StudentAdapter.java   # ListView adapter
├── DBHelper.java         # SQLite database helper
├── Student.java / Task.java   # data models
└── Tasks.java
```
