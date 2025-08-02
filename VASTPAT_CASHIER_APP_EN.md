
# VastPay Cashier

A Flutter-based mobile application for cashiers to manage invoices, orders, and reports for the VastPay payment system.

## 📱 Overview

VastPay Cashier is a comprehensive mobile application designed for cashiers to efficiently manage payment transactions, invoices, and generate reports. The app provides a user-friendly interface with Arabic and English localization support.

## ✨ Features

- **🔐 Authentication**: Secure login system for cashiers
- **💰 Invoice Management**: Add and manage invoices with custom keyboard input
- **📊 Reports**: Generate and view detailed transaction reports
- **📱 Real-time Updates**: Live invoice status updates via Pusher integration
- **🌐 Multi-language Support**: Arabic and English localization
- **📱 Cross-platform**: iOS and Android support
- **🎨 Modern UI**: Clean and intuitive user interface
- **🔄 Auto-updates**: In-app update functionality
- **📋 Terms & Privacy**: Built-in terms of service and privacy policy screens

## 🏗️ Architecture

This project follows **Clean Architecture** principles with **Riverpod** for state management:

```
lib/
├── blocs/           # Business Logic Layer
│   ├── events/      # UI Events
│   ├── models/      # Data Models
│   ├── providers/   # Riverpod Providers
│   ├── repositories/# Repository Interfaces
│   └── validators/  # Form Validation
├── data/            # Data Layer
│   ├── local/       # Local Data Sources
│   └── remote/      # Remote API Services
├── services/        # Service Layer
├── ui/              # Presentation Layer
│   ├── screens/     # App Screens
│   ├── widgets/     # Reusable Widgets
│   └── dialogs/     # Dialog Components
├── themes/          # App Theming
└── routes/          # Navigation
```

## 🛠️ Tech Stack

- **Framework**: Flutter 3.0+
- **State Management**: Riverpod
- **Navigation**: Go Router
- **Localization**: Easy Localization
- **Networking**: HTTP with custom interceptors
- **Real-time**: Pusher Channels
- **Storage**: Shared Preferences
- **Code Generation**: JSON Serializable, Build Runner
- **UI Components**: Custom widgets with Material Design

## 📋 Prerequisites

- Flutter SDK (>=3.0.0)
- Dart SDK (>=3.0.0)
- Android Studio / VS Code
- iOS development tools (for iOS builds)
- Git

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone <repository-url>
cd VastPay-Cashier
```

### 2. Install Dependencies

```bash
flutter pub get
```

### 3. Setup Environment

The app uses the following API endpoints:
- Base URL: `https://api.vast-pay.com/api/v1/`

### 4. Generate Code

```bash
# Generate JSON serializable code
flutter packages pub run build_runner build

# Generate assets
flutter packages pub run flutter_gen:generate

# Generate localization
flutter packages pub run easy_localization:generate
```

### 5. Run the App

```bash
# Debug mode
flutter run

# Release mode
flutter run --release
```

## 📱 App Screens

1. **Splash Screen**: App initialization and loading
2. **Login Screen**: Cashier authentication
3. **Add Invoice Screen**: Create new invoices with custom keyboard
4. **Reports Screen**: View transaction reports and analytics
5. **Invoice Status Screen**: Monitor invoice status in real-time
6. **More Screen**: Additional options and settings
7. **Terms & Privacy**: Legal information screens

## 🔧 Configuration

### API Configuration

Update API endpoints in `lib/data/remote/constants/end_points.dart`:

```dart
mixin AppEndpoints {
  static String baseUrl = "https://api.vast-pay.com/api/v1/";
  // ... other endpoints
}
```

### Localization

Supported languages:
- Arabic (default)
- English

Translation files are located in `assets/translations/`

### Fonts

The app uses custom Arabic fonts:
- **Tajawal**: Primary font family
- **Almarai**: Secondary font family
- **Noto Naskh Arabic**: Arabic text support

## 🏗️ Project Structure

```
VastPay-Cashier/
├── android/                 # Android-specific files
├── ios/                    # iOS-specific files
├── lib/                    # Main Flutter code
│   ├── blocs/             # Business logic
│   ├── data/              # Data layer
│   ├── services/          # API services
│   ├── ui/                # UI components
│   ├── themes/            # App theming
│   └── routes/            # Navigation
├── assets/                # App assets
│   ├── fonts/            # Custom fonts
│   ├── images/           # App images
│   └── translations/     # Localization files
└── test/                 # Unit tests
```

## 🧪 Testing

Run tests using:

```bash
# Run all tests
flutter test

# Run specific test file
flutter test test/test_login_screen.dart
```

## 📦 Building

### Android

```bash
# Debug APK
flutter build apk --debug

# Release APK
flutter build apk --release

# App Bundle
flutter build appbundle
```

### iOS

```bash
# Debug
flutter build ios --debug

# Release
flutter build ios --release
```

## 🔄 Scripts

The project includes several utility scripts:

- `scripts/buildrunner`: Code generation
- `scripts/localegen`: Localization generation
- `scripts/xcrun_android`: Android build helper
- `scripts/xcrun_ios`: iOS build helper

## 📄 Dependencies

### Core Dependencies

- `flutter_riverpod`: State management
- `go_router`: Navigation
- `easy_localization`: Internationalization
- `pusher_channels_flutter`: Real-time updates
- `flutter_screenutil`: Responsive design
- `shared_preferences`: Local storage

### Development Dependencies

- `build_runner`: Code generation
- `json_serializable`: JSON serialization
- `flutter_gen`: Asset generation
- `lint`: Code linting

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📝 License

This project is proprietary software. All rights reserved.

## 🆘 Support

For support and questions:
- Create an issue in the repository
- Contact the development team
- Check the project documentation

## 🔄 Version History

- **v1.0.7+8**: Current version with invoice management and real-time updates

---

**Note**: This is a production application for the VastPay payment system. Ensure proper security measures and testing before deployment.