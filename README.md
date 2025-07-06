# Secure-Bite

A Flutter application for food safety and nutrition information.

## Getting Started

This project is a Flutter application that helps users decode food labels and make healthier choices.

A few resources to get you started if this is your first Flutter project:

- [Lab: Write your first Flutter app](https://docs.flutter.dev/get-started/codelab)
- [Cookbook: Useful Flutter samples](https://docs.flutter.dev/cookbook)

For help getting started with Flutter development, view the
[online documentation](https://docs.flutter.dev/), which offers tutorials,
samples, guidance on mobile development, and a full API reference.

## Security Setup

### Important: API Keys and Sensitive Data

This project contains sensitive configuration files that should **NEVER** be committed to version control. The following files are automatically ignored by git:

- `android/app/google-services.json` - Firebase configuration for Android
- `lib/firebase_options.dart` - Firebase options with API keys
- `ios/Runner/GoogleService-Info.plist` - Firebase configuration for iOS
- Any `.env` files
- Certificate and key files (`.pem`, `.key`, `.p12`, `.keystore`)

### Setup Instructions

1. **Firebase Configuration:**
   - Copy `android/app/google-services.json.template` to `android/app/google-services.json`
   - Copy `lib/firebase_options.dart.template` to `lib/firebase_options.dart`
   - Replace the placeholder values with your actual Firebase project credentials

2. **Environment Variables:**
   - Create a `.env` file in the root directory if needed
   - Add any additional API keys or configuration values

3. **iOS Configuration (if applicable):**
   - Add your `GoogleService-Info.plist` to `ios/Runner/` directory

### Template Files

Template files are provided to show the required structure:
- `android/app/google-services.json.template`
- `lib/firebase_options.dart.template`

### Security Best Practices

- Never commit API keys or sensitive data to version control
- Use environment variables for different deployment environments
- Regularly rotate API keys and credentials
- Keep Firebase project settings secure
- Review the `.gitignore` file to ensure all sensitive files are excluded

## Features

- User authentication with Firebase
- Food label scanning and analysis
- Nutrition information display
- User profile management
- Dark/Light theme support
- Modern, aesthetic UI design

## Dependencies

This project uses the following key dependencies:
- Firebase Authentication
- Firebase Core
- SharedPreferences for theme persistence
- Google Fonts for typography
