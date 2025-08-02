# VastPay-App

A modern iOS restaurant menu and payment application built with SwiftUI, designed to provide seamless dining experiences with digital menus, ordering, and payment processing.

## 📱 Features

### Core Functionality
- **Digital Menu System** - Browse restaurant menus with categories and items
- **Order Management** - Add items to cart, customize orders, and track order status
- **Payment Processing** - Multiple payment methods including Apple Pay and card payments
- **QR Code Integration** - Scan QR codes to access restaurant menus
- **Real-time Updates** - Live order tracking and notifications using Pusher
- **Multi-language Support** - Arabic and English localization
- **Dark/Light Theme** - Customizable app appearance

### Payment Features
- Apple Pay integration
- Credit/Debit card payments
- Secure payment processing
- Invoice generation and PDF download
- Payment success tracking

### User Experience
- Intuitive SwiftUI interface
- Smooth animations and transitions
- Responsive design for different screen sizes
- Offline capability with network status checking
- Push notifications for order updates

## 🏗️ Architecture

### Project Structure
```
VastPay-App/
├── VastMenu/                    # Main iOS App
│   ├── App/                     # App entry point and configuration
│   ├── Model/                   # Data models and structures
│   ├── View/                    # SwiftUI views and components
│   ├── ViewModel/               # MVVM view models
│   ├── Services/                # API services and business logic
│   ├── Utils/                   # Utilities and helpers
│   ├── Payment/                 # Payment processing modules
│   └── Assets.xcassets/         # App resources
├── VastMenuAppClip/             # App Clip for QR code functionality
└── Configurations/              # Environment-specific configurations
```

### Design Patterns
- **MVVM (Model-View-ViewModel)** - Clean separation of concerns
- **Repository Pattern** - Data access abstraction
- **Dependency Injection** - Environment objects for state management
- **Protocol-Oriented Programming** - Flexible and testable code

## 🚀 Getting Started

### Prerequisites
- Xcode 15.0 or later
- iOS 15.0+ deployment target
- CocoaPods for dependency management
- Apple Developer Account (for App Store distribution)

### Installation

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd VastPay-App
   ```

2. **Install dependencies**
   ```bash
   pod install
   ```

3. **Open the workspace**
   ```bash
   open VastMenu.xcworkspace
   ```

4. **Configure environment**
   - Select the appropriate scheme (Dev/Prod)
   - Update configuration files in `Configurations/` directory
   - Add required API keys and endpoints

5. **Build and run**
   - Select your target device or simulator
   - Press `Cmd + R` to build and run

### Configuration

The app uses environment-specific configurations:

- **Development**: `Configurations/Dev/`
- **Production**: `Configurations/Prod/`

Key configuration variables:
- `BASE_URL` - API base URL
- `COOKIES_URL` - Cookies endpoint
- `PUSHER_KEY` - Real-time communication key

## 📦 Dependencies

### Core Dependencies
- **SwiftUI** - Modern iOS UI framework
- **Firebase** - Analytics, notifications, and crash reporting
- **PusherSwift** - Real-time communication
- **SDWebImageSwiftUI** - Image loading and caching

### Payment Dependencies
- **Apple Pay** - Native iOS payment processing
- Custom payment providers for card processing

### Development Dependencies
- **Sentry** - Error tracking and monitoring
- **UXCam** - User experience analytics (optional)

## 🔧 Development

### Code Style
- Follow Swift style guidelines
- Use meaningful variable and function names
- Add comments for complex logic
- Maintain consistent indentation

### File Organization
- Group related files in appropriate directories
- Use clear naming conventions
- Separate concerns (UI, business logic, data)

### Testing
- Unit tests for view models and services
- UI tests for critical user flows
- Integration tests for API services

## 📱 App Features

### Main Views
- **HomeView** - Restaurant menu and categories
- **CartView** - Shopping cart and checkout
- **OrderDetailsView** - Order tracking and status
- **PaymentView** - Payment method selection
- **InvoiceView** - Order receipts and history

### Key Components
- **Custom UI Components** - Reusable SwiftUI components
- **Network Layer** - Robust API communication
- **Localization** - Multi-language support
- **Theme System** - Customizable appearance

## 🔐 Security

- Secure API communication with HTTPS
- Token-based authentication
- Secure payment processing
- Data encryption for sensitive information
- Privacy compliance with iOS guidelines

## 📊 Analytics & Monitoring

- **Firebase Analytics** - User behavior tracking
- **Sentry** - Error monitoring and crash reporting
- **Push Notifications** - Order updates and promotions
- **Network Monitoring** - Connection status tracking

## 🌐 Localization

The app supports multiple languages:
- **English** - Primary language
- **Arabic** - RTL support with custom fonts

Localization files are located in:
- `en.lproj/Localizable.strings`
- `ar.lproj/Localizable.strings`

## 📱 App Clip

The project includes an App Clip (`VastMenuAppClip`) that provides:
- Quick access via QR codes
- Lightweight menu browsing
- Seamless transition to full app

## 🚀 Deployment

### App Store Distribution
1. Configure signing certificates
2. Update version and build numbers
3. Archive the project
4. Upload to App Store Connect

### CI/CD
- **Codemagic** - Automated builds and deployment
- Configuration file: `codemagic.yaml`

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Add tests if applicable
5. Submit a pull request

## 📄 License

This project is proprietary software. All rights reserved.

## 📞 Support

For technical support or questions:
- Create an issue in the repository
- Contact the development team
- Check the documentation

## 🔄 Version History

- **v1.0.0** - Initial release with core functionality
- **v1.1.0** - Added payment processing
- **v1.2.0** - Enhanced UI and performance improvements
- **v1.3.0** - Added App Clip and QR code functionality

---

**Built with ❤️ using SwiftUI and modern iOS development practices** 