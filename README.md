# TapU - Smart Attendance System

[![Flutter](https://img.shields.io/badge/Flutter-%2302569B.svg?style=flat-square&logo=Flutter&logoColor=white)](https://flutter.dev)
[![Dart](https://img.shields.io/badge/Dart-%230175C2.svg?style=flat-square&logo=Dart&logoColor=white)](https://dart.dev)
[![License](https://img.shields.io/badge/License-MIT-green.svg?style=flat-square)](LICENSE)

## 📋 Overview

**TapU** is an innovative attendance tracking system developed as a final project for CIS 228 - Mobile Application Development. It revolutionizes the traditional roll call process by leveraging mobile sensors and NFC (Near Field Communication) technology to enable seamless, contactless attendance marking.

Instead of time-consuming manual roll calls, TapU allows students to simply **"tap"** their student ID cards or devices against an NFC reader, providing teachers with instant, accurate attendance records.

### Key Features

- ✅ **NFC-Based Attendance** - Quick tap-to-mark attendance system
- 📱 **Mobile-First Design** - Built with Flutter for cross-platform compatibility
- 🔄 **Real-Time Sync** - Instant attendance updates for teachers
- 👥 **Multi-User Support** - Separate interfaces for teachers and students
- 📊 **Analytics Dashboard** - Track attendance patterns and generate reports
- 🔒 **Secure** - Built with security best practices for student data protection
- 📡 **Sensor Integration** - Utilizes device sensors for enhanced functionality

## 🛠 Tech Stack

- **Frontend**: Flutter (Dart)
- **Native Code**: C++, C (for sensor handling and NFC integration)
- **Build System**: CMake
- **Platform Support**: iOS & Android
- **Architecture**: Model-View-Controller (MVC)

### Language Composition
- Dart: 76.9%
- C++: 11.5%
- CMake: 9.1%
- Swift: 1.2%
- C: 0.6%
- HTML: 0.6%

## 📦 Prerequisites

Before you begin, ensure you have the following installed:

- [Flutter SDK](https://flutter.dev/docs/get-started/install) (latest stable version)
- [Dart SDK](https://dart.dev/get-dart) (comes with Flutter)
- [Android Studio](https://developer.android.com/studio) or [Xcode](https://developer.apple.com/xcode/) (for iOS)
- NFC-enabled device (for full functionality)

### System Requirements

- **Android**: API level 21 or higher
- **iOS**: iOS 11.0 or higher
- **NFC**: Device must support NFC (most modern smartphones do)

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/N0Kzs/TapU.git
cd TapU
```

### 2. Install Dependencies

```bash
flutter pub get
```

### 3. Build and Run

#### For Android
```bash
flutter run -d android
```

#### For iOS
```bash
flutter run -d ios
```

#### For Web (if supported)
```bash
flutter run -d chrome
```

### 4. Run on Physical Device

Connect your NFC-enabled device and run:
```bash
flutter run
```

## 📖 Project Structure

```
TapU/
├── lib/
│   ├── main.dart              # App entry point
│   ├── screens/               # UI screens
│   ├── models/                # Data models
│   ├── services/              # Business logic & NFC services
│   ├── widgets/               # Reusable widgets
│   └── utils/                 # Utility functions
├── android/                   # Android native code
├── ios/                       # iOS native code
├── test/                      # Unit and integration tests
├── pubspec.yaml              # Flutter dependencies
└── README.md
```

## 🎯 Main Components

### Teacher Dashboard
- View class attendance summaries
- Mark attendance manually if needed
- Generate attendance reports
- Manage student lists

### Student Interface
- Simple tap-to-mark attendance
- View personal attendance history
- Receive notifications

### NFC Module
- Reads student ID cards/devices
- Communicates with backend for verification
- Handles NFC communication errors gracefully

## 🔧 Configuration

### NFC Permissions

#### Android (`android/app/src/main/AndroidManifest.xml`)
```xml
<uses-permission android:name="android.permission.NFC" />
<uses-feature android:name="android.hardware.nfc" android:required="false" />
```

#### iOS (`ios/Runner/Info.plist`)
```xml
<key>NFCReaderUsageDescription</key>
<string>We need NFC access to read your student ID</string>
```

## 🧪 Testing

Run tests with:

```bash
flutter test
```

Run specific test file:
```bash
flutter test test/services/nfc_service_test.dart
```

## 📝 Development

### Formatting Code
```bash
flutter format lib/ test/
```

### Analyzing Code
```bash
flutter analyze
```

### Building for Production

#### Android
```bash
flutter build apk --release
```

#### iOS
```bash
flutter build ios --release
```

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 👨‍💻 Author

**N0Kzs** - [GitHub Profile](https://github.com/N0Kzs)

## 📞 Support

For issues, questions, or suggestions, please:
- Open an [issue](https://github.com/N0Kzs/TapU/issues) on GitHub
- Contact the project maintainer

## 🎓 Course Information

- **Course**: CIS 228 - Mobile Application Development
- **Project Type**: Final Project
- **Focus**: Business Integration using smartphone sensors with Flutter

## 🚦 Status

- Development Status: Active
- Last Updated: June 2025
- Maintained by: N0Kzs

---

**Made with ❤️ by N0Kzs**
