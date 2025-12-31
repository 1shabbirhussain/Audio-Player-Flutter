# Flutter Mobile App 🎵

A feature-rich Flutter mobile application built with modern architecture and best practices. This project demonstrates a clean, scalable approach to Flutter development with state management, local storage, and multimedia capabilities.

## 📱 Screenshots

<!-- Add your screenshots here -->
<!-- Example:-->

<div align="center">
<img width="250"  alt="Screenshot_1767175247" src="https://github.com/user-attachments/assets/8990f7bc-ae97-4214-90b3-689c5e8f4736" />
<img width="250"  alt="Screenshot_1767175249" src="https://github.com/user-attachments/assets/aa5a4640-cf52-4cc2-acbd-7a2da660c179" />
<img width="250"  alt="Screenshot_1767175215" src="https://github.com/user-attachments/assets/5c95f969-d59d-4ede-9f4c-38b1583b7943" />
<img width="250"  alt="Screenshot_1767175255" src="https://github.com/user-attachments/assets/0da0d45d-27fa-4b0a-82c7-949cf2381c05" />
<img width="250"  alt="Screenshot_1767175218" src="https://github.com/user-attachments/assets/76e85ac2-48ce-468d-8093-aa9f71306b5f" />
<img width="250"  alt="Screenshot_1767175267" src="https://github.com/user-attachments/assets/304e34d9-3892-47ef-a569-eda2f98fa1c0" />
<img width="250"  alt="Screenshot_1767175260" src="https://github.com/user-attachments/assets/2fc39291-985c-460d-8b6e-c79b3bf937fd" />
<img width="250"  alt="Screenshot_1767175225" src="https://github.com/user-attachments/assets/7fb4c47f-34e8-485a-a017-a5c192421719" />
<img width="250"  alt="Screenshot_1767175227" src="https://github.com/user-attachments/assets/0fc85a42-a1b3-4afd-9812-df75505eb73a" />
<img width="250"  alt="Screenshot_1767175246" src="https://github.com/user-attachments/assets/59bebc65-47fc-41a9-8bb0-0464daf9d842" />

</div>

## ✨ Features

- 🎨 **Dynamic Theming** - Light and dark mode support with persistent theme preferences
- 🎵 **Audio Playback** - Full-featured audio player with background playback support
- 📂 **Media Management** - Query and manage audio files from device storage
- 🔔 **Media Notifications** - Rich media notifications with playback controls
- 💾 **Local Storage** - Persistent data storage using GetStorage
- 🔄 **State Management** - Reactive state management with GetX
- 📱 **Responsive UI** - Adaptive layouts for different screen sizes
- 🎯 **Permission Handling** - Runtime permission requests for storage and notifications
- 📤 **Share Functionality** - Share content with other apps
- ⚡ **Haptic Feedback** - Vibration support for enhanced user experience

## 🏗️ Architecture

This project follows clean architecture principles with separation of concerns:

```
lib/
├── bindings/          # Dependency injection bindings
├── config/
│   └── theme/         # Theme configuration and styles
├── controllers/       # GetX controllers for state management
├── models/            # Data models
├── routes/            # Navigation and route definitions
├── screens/           # UI screens/pages
├── services/          # Business logic and API services
├── utils/             # Utility functions and constants
├── widgets/           # Reusable UI components
└── main.dart          # Application entry point
```

## 🚀 Getting Started

### Prerequisites

- **Flutter SDK**: Version 3.0 or higher
- **Dart SDK**: Version 3.0 or higher
- **Android Studio** / **VS Code** with Flutter plugins
- **Android SDK**: API Level 21 (Android 5.0) or higher
- **iOS**: iOS 12.0 or higher (for iOS builds)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/flutter_mobile_app.git
   cd flutter_mobile_app
   ```

2. **Install dependencies**
   ```bash
   flutter pub get
   ```

3. **Run the app**
   ```bash
   # For debug mode
   flutter run
   
   # For release mode
   flutter run --release
   ```

## 📦 Dependencies

### Core Dependencies
- [`get: ^4.7.3`](https://pub.dev/packages/get) - State management, routing, and dependency injection
- [`get_storage: ^2.1.1`](https://pub.dev/packages/get_storage) - Fast, lightweight local storage

### Media & Audio
- [`just_audio: ^0.9.42`](https://pub.dev/packages/just_audio) - Audio playback functionality
- [`audio_service: ^0.18.17`](https://pub.dev/packages/audio_service) - Background audio service
- [`audio_session: ^0.1.23`](https://pub.dev/packages/audio_session) - Audio session management
- [`on_audio_query: ^2.9.0`](https://pub.dev/packages/on_audio_query) - Query audio files from device

### Utilities
- [`path_provider: ^2.1.5`](https://pub.dev/packages/path_provider) - Access to filesystem directories
- [`permission_handler: ^11.3.1`](https://pub.dev/packages/permission_handler) - Runtime permission handling
- [`share_plus: ^10.1.2`](https://pub.dev/packages/share_plus) - Share content functionality
- [`device_info_plus: ^11.2.0`](https://pub.dev/packages/device_info_plus) - Device information
- [`sqflite: ^2.4.1`](https://pub.dev/packages/sqflite) - SQLite database support
- [`vibration: ^2.0.0`](https://pub.dev/packages/vibration) - Haptic feedback

### UI
- [`cupertino_icons: ^1.0.8`](https://pub.dev/packages/cupertino_icons) - iOS-style icons

## 🔧 Configuration

### Android Setup

The app requires minimum SDK version 21 (Android 5.0). Configuration is in `android/app/build.gradle.kts`:

```kotlin
minSdk = 21
targetSdk = 34
compileSdk = 34
```

### Permissions

Required permissions are automatically handled by the plugins. Key permissions include:
- Storage access (for audio files)
- Notification access (for media controls)
- Vibration (for haptic feedback)

## 📱 Build Instructions

### Android APK

```bash
# Build debug APK
flutter build apk --debug

# Build release APK
flutter build apk --release

# Build app bundle (for Google Play)
flutter build appbundle --release
```

### iOS

```bash
# Build for iOS
flutter build ios --release
```

## 🎨 Theming

The app supports dynamic theming with custom color schemes and styles. Theme preferences are persisted using GetStorage and managed through the ThemeController.

**Features:**
- Light and dark mode support
- Custom color palettes
- Glassmorphic UI elements
- Neon-styled buttons and accents
- Smooth theme transitions

## 🧪 Testing

```bash
# Run all tests
flutter test

# Run tests with coverage
flutter test --coverage
```

## 📝 Project Structure

```
flutter_mobile_app/
├── android/              # Android native code
├── ios/                  # iOS native code
├── lib/                  # Dart source code
│   ├── bindings/        # GetX dependency injection
│   ├── config/          # App configuration
│   ├── controllers/     # State management
│   ├── models/          # Data models
│   ├── routes/          # Navigation
│   ├── screens/         # UI screens
│   ├── services/        # Business logic
│   ├── utils/           # Helpers & constants
│   ├── widgets/         # Reusable components
│   └── main.dart        # Entry point
├── assets/              # Images, fonts, icons
├── test/                # Test files
└── pubspec.yaml         # Dependencies
```

## 🎯 Key Features Breakdown

### Audio Player
- Background playback with audio service
- Media notification controls
- Play, pause, skip, seek functionality
- Playlist support
- Audio visualization
- Beat pulse animations

### Library Management
- Query audio files from device
- Create and manage playlists
- Search and filter audio files
- Sort by title, artist, duration

### UI/UX
- Glassmorphic design elements
- Smooth animations and transitions
- Mini player widget
- Custom progress bars
- Responsive layouts

## 🤝 Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

### Code Style

- Follow [Effective Dart](https://dart.dev/guides/language/effective-dart) guidelines
- Use meaningful variable and function names
- Add comments for complex logic
- Format code using `flutter format .`
- Run `flutter analyze` before committing

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 👥 Authors

- Your Name - [@yourusername](https://github.com/yourusername)

## 🙏 Acknowledgments

- Flutter team for the amazing framework
- GetX community for the powerful state management solution
- All contributors and package maintainers

## 📧 Support

For support, email your.email@example.com or open an issue in the repository.

## 🔮 Roadmap

- [ ] Add cloud sync capabilities
- [ ] Implement equalizer
- [ ] Add lyrics support
- [ ] Sleep timer functionality
- [ ] Cross-fade between tracks
- [ ] Home screen widgets
- [ ] Car mode interface
- [ ] Podcast support

## 📊 Project Status

This project is currently in active development. Features and APIs may change.

---

**Note**: Replace placeholder values (repository URL, author name, email) with your actual information before publishing to GitHub. Don't forget to add your screenshots in the Screenshots section!
