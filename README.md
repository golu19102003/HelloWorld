<img width="371" height="795" alt="image" src="https://github.com/user-attachments/assets/2b0acd1d-4408-4b08-9b8d-1e92b3a794cf" />

# HelloWorldApp
HelloWorldApp is a basic Android application designed to display a simple "Hello, World!" message on the screen. This project serves as an introductory example for beginners starting with Android development, covering essential concepts like activity lifecycle, XML layouts, UI components, and basic project structure.

## ✨ Features:
✔ Simple UI
Displays a clear, centered message: “Hello, World!”

✔ Beginner-Friendly
Provides a clean and minimal codebase ideal for learning Android development basics.

✔ Activity Lifecycle
Introduces the concept of an Activity (MainActivity.java) as the main entry point.

✔ XML Layout
Shows how the UI is created using Android’s XML layout system.

✔ Easy to Modify
You can change the text message, styling, colors, or add more controls easily.

## 🛠️ Build Requirements:

Minimum SDK: API 21 (Android 5.0 Lollipop)

Target SDK: API 33+

Programming Language: Java 8 or higher

Development Environment: Android Studio (recommended)

## 📁 Project Structure:

The project follows a standard Android application format:

HelloWorldApp/
├── app/
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/com/example/helloworldapp/MainActivity.java   // Main logic
│   │   │   ├── res/layout/activity_main.xml                       // UI layout
│   │   │   ├── AndroidManifest.xml                                // App manifest

## 🚀 Installation & Setup:
**1.** Create or Import the Project
Open Android Studio

Select New Project → Empty Activity

Enter:

Application Name: HelloWorldApp

Package Name: com.example.helloworldapp

**2.** Sync with Gradle

Android Studio will automatically sync, or click:
File → Sync Project with Gradle Files

**3.** Build & Run

-Connect an Android device OR launch an emulator

-Press the Run (▶) button

-The app will install and display "Hello, World!"

## 💡 Usage:

Once launched, the app shows:
📍 A centered “Hello, World!” message
on a clean white screen.

This is the most basic Android application and serves as the starting point for building more complex apps.

## 📝 Key Implementation Details:
### 📌 MainActivity.java

This file contains the logic that displays the layout and acts as the entry point to the application.

MainActivity.java (Java)
package com.example.helloworldapp;

import android.os.Bundle;
import androidx.appcompat.app.AppCompatActivity;

/**
 * MainActivity is the primary entry point of the HelloWorldApp.
 * It loads the layout and displays the "Hello, World!" message.
 */
public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);

        // Set the UI layout for this Activity.
        setContentView(R.layout.activity_main);
    }
}

### 📌 activity_main.xml

This file defines the visual interface shown to the user.

<?xml version="1.0" encoding="utf-8"?>
<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:orientation="vertical"
    android:gravity="center"
    android:background="#FFFFFF">

    <TextView
        android:id="@+id/helloText"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Hello, World!"
        android:textSize="24sp"
        android:textColor="#000000" />
</LinearLayout>

### 📌 AndroidManifest.xml

Includes application configuration, theme, and activity declaration.

<application
    android:allowBackup="true"
    android:label="HelloWorldApp"
    android:theme="@style/Theme.AppCompat.Light.NoActionBar">

    <activity
        android:name=".MainActivity"
        android:exported="true">
        <intent-filter>
            <action android:name="android.intent.action.MAIN"/>
            <category android:name="android.intent.category.LAUNCHER"/>
        </intent-filter>
    </activity>
</application>

## 🧪 Test Cases:
-Scenario	Expected Output
-Launch app	“Hello, World!” displayed in center ✔
-Rotate device	Layout adjusts automatically ✔
-App in background & resume	Message remains visible ✔
-App restart	Loads message instantly ✔

## 🚧 Possible Enhancements:

You can extend this project by:

🎨 Changing text size, color, or font

🌈 Adding background images or gradients

🔘 Adding buttons, inputs, or navigation

🌐 Moving to multi-screen apps using Activities/Fragments

💬 Adding user interaction events

🛠 Switching to Kotlin for modern development

## 🤝 Contributing:

Feel free to customize, fork, or improve this project.
Pull requests are welcome!

## 📄 License:

This project is open-sourced under the MIT License.
