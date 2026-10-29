# Word Guessing Game – Hybrid Android Application

## About the Project

The **Word Guessing Game** is a web-based game converted into an Android mobile application using a hybrid app development approach. The application uses Android WebView to display and run the existing website within a native Android application.

This project was developed as part of the **Mobile Application Development (MAD) assignment**.

## Objectives

- Convert an existing web-based project into a mobile application.
- Use web technologies to develop the application's interface and functionality.
- Integrate the website into an Android application using WebView.
- Build an APK that can be installed on Android devices.

## Technologies Used

- **HTML** – Structure of the game interface.
- **CSS** – Styling and layout.
- **JavaScript** – Game logic and interactivity.
- **Java** – Android activity implementation.
- **Android WebView** – Displays the website within the Android application.
- **Android Studio** – Development and APK generation.

## Project Structure

```text
WordGuessingGame/
├── Website Source Code/
│   ├── index.html
│   ├── index.css
│   ├── index.js
│   └── img/
│
├── Android Project/
│   └── app/
│       └── src/
│           └── main/
│               ├── assets/
│               │   ├── index.html
│               │   ├── index.css
│               │   ├── index.js
│               │   └── img/
│               ├── java/
│               │   └── com/example/wordguessinggame/
│               │       └── MainActivity.java
│               └── AndroidManifest.xml
│
└── README.md
```

*Note: The folder names shown above illustrate the organization of the project. The actual uploaded folder structure may differ.*

## Hybrid Application Implementation

The Android application uses WebView to load the local `index.html` file stored in the Android project's assets directory.

The HTML, CSS, JavaScript, and image files are packaged with the application, allowing the web-based interface and game logic to run inside the Android app.

The main Android activity initializes WebView and loads the local webpage using:

```java
webView.loadUrl("file:///android_asset/index.html");
```

This approach reuses the existing web application instead of rebuilding the entire interface using native Android layouts.

## How to Run the Project

### Option 1: Install the APK

1. Download the APK file from this repository.
2. Transfer it to an Android device if necessary.
3. Allow installation from the relevant source if Android requests permission.
4. Install and open the application.

### Option 2: Run Using Android Studio

1. Download or clone this repository.
2. Extract the Android project ZIP file if it is provided separately.
3. Open the Android project in Android Studio.
4. Allow Gradle synchronization to complete.
5. Run the application on an Android emulator or a physical Android device.

## Deliverables

The repository includes the following assignment deliverables:

- Original website source code.
- Complete Android Studio project source code.
- Compiled Android APK file.
- Project documentation.

## Learning Outcomes

- Understanding hybrid mobile application development.
- Integrating web technologies with Android.
- Using WebView to display local web content.
- Packaging a web-based application as an installable Android application.
- Building and testing an Android application using Android Studio.

## Conclusion

This project demonstrates how an existing web-based Word Guessing Game can be converted into an Android application using a WebView-based hybrid approach. It reuses HTML, CSS, and JavaScript while providing an Android application package for installation and testing.

---

**Assignment:** Mobile Application Development (MAD)  
**Project:** Word Guessing Game – Hybrid Android Application
