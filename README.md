# CareSyncApp
CareSync App
Contributors
Danielle Clowden
Expertise: Full-Stack Development, API Integration
Contributions: Backend architecture, Fitbit API integration, database schema design
Ariana Singh 
Expertise: Frontend Development, User Interface Design, Documentation
Contributions: Developed app UI using Java, ensured seamless user experience, contributed to API integration
Jeremy Persaud
Expertise: Quality Assurance, Documentation, UI Design 
Contributions: Assisted with testing and debugging, contributed to project documentation

User Guide
Google Drive Link
Access the app demo video and APK file via this public Google Drive link: 
App Installation and Usage
Download the App
Download the APK file from the Google Drive link above.
Transfer the APK to your Android device.
Install the App
Enable "Install from Unknown Sources" on your Android device:
Go to Settings > Security > Unknown Sources and enable it.
Tap on the APK file to begin installation.
Set Up the App
Open the app and create an account using your email.
Connect your Fitbit or compatible wearable device.
Configure medication schedules and caregiver profiles.
Use the App
Access health metrics, schedule reminders, and track real-time patient health data.
Testing Strategies and Results
Unit Testing
Test: Validate that medication reminders trigger at the scheduled time.
Result: Notifications are delivered as expected without delays.
Integration Testing
Test: Ensure Fitbit API syncs health data to the app dashboard correctly.
Result: Health metrics (e.g., heart rate, step count) appear accurately.
System Testing
Test: Verify app performance with multiple caregivers linked to one patient.
Result: Smooth functionality without lag or errors.

Technology Stack
Software Requirements
Development Tools: Android Studio, Figma, GitHub
Programming Languages: Java, React

Setup Guide
Development Environment Setup
Clone the Repository:
https://github.com/asing200/CareSync.git
cd caresync
Open in Android Studio:
Launch Android Studio.
Open the project directory.
Configure API Keys:
Obtain Fitbit API credentials and configure them in the strings.xml file:
<string name="fitbit_api_key">YOUR_API_KEY</string>
<string name="fitbit_api_secret">YOUR_API_SECRET</string>
Run the App:
Connect an Android device or launch an emulator in Android Studio.
Click Run to build and deploy the app.
Production Deployment
Generate a signed APK in Android Studio for distribution.
Test the APK on various devices to ensure compatibility.

Features and Technical Implementation
Real-Time Health Monitoring
Implementation: Integrated Fitbit API to fetch health metrics like heart rate, step count, and sleep data. Displayed data dynamically on the dashboard.
Medication Reminders
Implementation: Developed a notification system using Android's AlarmManager API to send push notifications for reminders.
Caregiver Dashboard
Implementation: Designed using RecyclerView to list multiple patients and display key metrics.

Packages and APIs
APIs Used
Fitbit API
Reason: To fetch real-time health metrics from wearable devices.
Endpoints:
GET /1/user/-/activities/steps/date/today/1d.json
GET /1/user/-/sleep/date/today.json
Authentication: OAuth 2.0
Packages Used
Android Jetpack Components: For efficient app architecture and lifecycle management.
Retrofit: To simplify API calls and handle JSON parsing.
Room Database: To store user data locally.
React: For building responsive and reusable UI components in some parts of the application.
