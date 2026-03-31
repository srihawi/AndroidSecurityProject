Android Security Project
A comprehensive demonstration of security best practices for Android application development. This project serves as a reference for implementing robust security layers, protecting sensitive user data, and hardening applications against common vulnerabilities.

🔒 Key Security Features
Data Encryption at Rest: Implementation of the Jetpack Security (EncryptedSharedPreferences) library to ensure that local data is stored using AES-256 encryption.

Secure Networking: Implementation of Certificate Pinning and Network Security Configuration to prevent Man-in-the-Middle (MitM) attacks.

Code Obfuscation: Pre-configured ProGuard/R8 rules to minify code and obfuscate sensitive logic, making reverse engineering significantly more difficult.

Biometric Authentication: Integration of the BiometricPrompt API for secure, hardware-backed user identity verification.

Root & Emulator Detection: Logic to identify if the app is running in a compromised environment, allowing for proactive security measures.

🛠️ Tech Stack
Language: Kotlin / Java

Build System: Gradle

Security Libraries: Google Tink, Jetpack Security, Biometric Library.

Static Analysis: Integrated with Lint and specialized security scanning tools.

🚀 Getting Started
Prerequisites
Android Studio Hedgehog or newer.

Android SDK Level 23 (Marshmallow) or higher.

Installation
Clone the repository:

Bash
git clone https://github.com/srihawi/AndroidSecurityProject.git
cd AndroidSecurityProject
Build the project:
Open the project in Android Studio and sync the Gradle files.

Run the App:
Select a physical device or emulator and click the 'Run' icon.

📋 Security Checklist Implemented
[x] Use of android:allowBackup="false" in Manifest.

[x] Secure WebView configurations (disabling JavaScript if not needed).

[x] Input validation to prevent SQL Injection and XSS.

[x] Handling of sensitive data in memory (clearing CharArrays).
