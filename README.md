# Expense Tracker

A cross-platform expense tracking app built with Flutter. Track your daily expenses with a beautiful, responsive UI for Android, iOS, web, and desktop.

## Features

- Add, view, and delete expenses
- Category icons and formatted dates
- Responsive Material Design UI
- Works on Android, iOS, web, and desktop

## Requirements

- [Flutter SDK](https://flutter.dev/docs/get-started/install) (3.0 or higher recommended)
- Android Studio or Xcode (for mobile development)
- CocoaPods (for iOS, install with `sudo gem install cocoapods`)

## Getting Started

1. **Clone the repository:**
   ```sh
   git clone <repo-url>
   cd expense_tracker
   ```
2. **Install dependencies:**
   ```sh
   flutter pub get
   ```
3. **Run on Android:**
   ```sh
   flutter run -d <android-device-id>
   ```
4. **Run on iOS:**

   ```sh
   flutter create .
   cd ios
   pod install
   cd ..
   flutter run -d <ios-device-id>
   ```

   > If you get a codesigning error, open `ios/Runner.xcworkspace` in Xcode and ensure a valid Team and signing certificate are selected under Signing & Capabilities.

5. **Run on Web:**
   ```sh
   flutter run -d chrome
   ```

## Troubleshooting

- **No Podfile found:**
  - Run `flutter create --platforms=ios .` from the project root to regenerate iOS files.
- **Codesigning errors on iOS:**
  - Open the project in Xcode, select a valid Team, and enable automatic signing.
- **Permission denied or read-only errors:**
  - Ensure you own the Flutter SDK and project files: `sudo chown -R $USER: <flutter-sdk-path>`
  - Make files writable: `sudo chmod -R u+w <flutter-sdk-path>`
- **Emulator/Simulator performance issues:**
  - Close other apps, lower emulator RAM, or use a physical device.

## Resources

- [Flutter Documentation](https://docs.flutter.dev/)
- [Dart Documentation](https://dart.dev/guides)

---

_Happy expense tracking!_
