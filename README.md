# Mobile application

This project was developed during an internship as part of a mobile development practice. The goal was to design and implement a functional mobile app focused on allowing the user to order coffee in advance, choose a convenient arrival time and pick up the order without leaving the car.

## Features

 * **Premium UI:** A visually attractive, intuitive, and well-designed interface for an enhanced user experience.
 * **Popular Coffees:**
   * Users can view coffee ratings.
   * Users can choose from different coffee sizes.
   * Users can add their preferred coffee to the shopping cart.
 * **Shopping Cart Screen:**
   * See all items added to the cart with their individual prices.
      * Check the total cost of all items.
      * View the delivery charges applied to the order.
      * View the total tax on the items.
      * See the overall price for the entire order.

## Screenshots

<div align="center">
  <img src="https://github.com/user-attachments/assets/904d77b1-78f1-41b5-ab43-f6c1e6934bd8" width="200" alt="Coffee Shop Image">
  <img src="https://github.com/user-attachments/assets/7dd2f990-ee7f-4f17-a626-b9ef1cf19a52" width="200" alt="Coffee Shop Image">
  <img src="https://github.com/user-attachments/assets/7595290a-7b03-4962-9291-9c10039a0f92" width="200" alt="Coffee Shop Image">
  <img src="https://github.com/user-attachments/assets/7ade6963-ef29-434e-b9ed-559ffaf7b376" width="200" alt="Coffee Shop Image">
  <br>
</div>

## Getting Started
The project was developed as part of our mobile development practice. Below are the steps to get the project up and running.

#### 1. [Install Android Studio](https://developer.android.com/studio)

#### 2. Clone the Repository

```
$ git clone https://github.com/practiceFinalProject/CoffeePractice.git
$ cd CoffeePractice/
```

#### 3. Setup Firebase Realtime Database

1. Create a Firebase Project:
    - Go to the [Firebase Console](https://console.firebase.google.com/) and create a new project.
2. Enable Firebase Realtime Database:
      - Click on Realtime Database from the left-hand menu.
      - Click on "Create Database."
      - Choose "Start in test mode" for initial setup and click "Enable."
3. Add Data to Realtime Database:
    - Go to the Firebase Realtime Database in the console.
    - Click on the three dots in the upper right corner and select Import JSON.
    - Choose the `database_firebase.json` file and import it to populate the database with initial data.

#### 4. Configure Firebase for Android

1. Create an Android App in Firebase:
    - In the Firebase console, go to **Project settings**.
    - Under "Your apps," select **Add app** and choose **Android**.
    - Enter your package name.
2. Add SHA-1 Key:
    - Run the following command to get your SHA-1 key:
      
      ```
      keytool -exportcert -list -v -alias androiddebugkey -keystore ~/.android/debug.keystore
      ```
    - In the Firebase console, under the Android app settings, add your SHA-1 key by clicking "Add Fingerprint."

#### 5. Add Dependencies
  - Verify and add the latest versions of Firebase Realtime Database, Lifecycle and Gson dependencies to your project.
  - For detailed instructions on setting up Firebase refer to the [Firebase Realtime Database Setup Guide](https://firebase.google.com/docs/database/android/start).
  - Ensure View Binding is enabled. If not, add the following inside the `android` block in your `build.gradle` file (Module: app):
    
    ```
    buildFeatures{
        viewBinding = true
    }
    ```
  - Sync your project with Gradle to ensure all dependencies are correctly added.

#### 6. Final Step
  - Build and run the app on your Android device or emulator.


