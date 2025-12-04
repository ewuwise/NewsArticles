# 📰 NewsArticles - React Native News App

<div align="center">

![React Native](https://img.shields.io/badge/React_Native-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Expo](https://img.shields.io/badge/Expo-000020?style=for-the-badge&logo=expo&logoColor=white)
![Redux](https://img.shields.io/badge/Redux-764ABC?style=for-the-badge&logo=redux&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-blue.svg?style=for-the-badge)

**A feature-rich mobile news application to discover, save, and create news articles**

[Features](#-features) • [Screenshots](#-screenshots) • [Installation](#-installation) • [Usage](#-usage) • [Project Structure](#-project-structure)

</div>

## 🚀 Overview

NewsArticles is a modern React Native application that allows users to browse news across different categories, save their favorite articles, and even create their own custom news content. Built with Expo for cross-platform compatibility and Redux for state management, this app provides a seamless news reading experience on iOS, Android, and Web.

## ✨ Features

### 📰 **News Discovery**
- **Categorized Feed**: Browse articles across Technology, Sports, Business, Entertainment, Science, and Health
- **Smart Filtering**: Horizontal scrollable category bar for instant content filtering
- **Rich Media Display**: Article thumbnails with responsive grid layout
- **Dynamic Content**: Articles with images, titles, descriptions, and metadata

### ❤️ **Personal Management**
- **Favorites System**: Save and organize favorite articles with heart icons
- **Local Storage**: Persistent favorites using Redux
- **Custom Articles**: Create, edit, and delete your own news content using AsyncStorage
- **Quick Access**: Easy navigation to saved content

### 🎨 **User Experience**
- **Smooth Navigation**: Seamless transitions between screens using React Navigation
- **Responsive Design**: Adapts to different screen sizes with `react-native-responsive-screen`
- **Modern UI**: Clean interface with attractive animations and visual feedback
- **Intuitive Controls**: Easy-to-use buttons and gestures

### 🔧 **Technical Excellence**
- **Cross-Platform**: Works on iOS, Android, and Web
- **State Management**: Global favorites management using Redux Toolkit
- **Local Persistence**: User data saved locally
- **Optimized Performance**: Efficient rendering with FlatList and memoization

## 📸 Screenshots

| Welcome Screen | Home Screen | Article Details |
|:--------------:|:-----------:|:---------------:|
| ![Welcome](https://via.placeholder.com/300x600/6439FF/FFFFFF?text=Welcome) | ![Home](https://via.placeholder.com/300x600/8A2BE2/FFFFFF?text=News+Feed) | ![Details](https://via.placeholder.com/300x600/9400D3/FFFFFF?text=Article) |

| Favorites | My Articles | Create Article |
|:---------:|:-----------:|:--------------:|
| ![Favorites](https://via.placeholder.com/300x600/FF6B6B/FFFFFF?text=Favorites) | ![My Articles](https://via.placeholder.com/300x600/4ECDC4/FFFFFF?text=My+News) | ![Create](https://via.placeholder.com/300x600/45B7D1/FFFFFF?text=Create) |

## 🛠️ Tech Stack

- **Frontend Framework**: React Native 0.72.6
- **Development Platform**: Expo 49
- **Navigation**: React Navigation 6
- **State Management**: Redux Toolkit 2
- **Local Storage**: AsyncStorage
- **Responsive Design**: react-native-responsive-screen
- **Animations**: React Native Reanimated
- **Styling**: React Native StyleSheet

## 📦 Installation

### Prerequisites
- Node.js (v16 or higher)
- npm or yarn
- Expo CLI (`npm install -g expo-cli`)
- iOS Simulator (for iOS development) or Android Studio (for Android)

### Step-by-Step Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/ewuwise/NewsArticles.git
   cd NewsArticles
   ```

2. **Install dependencies**
   ```bash
   npm install
   # or
   yarn install
   ```

3. **Start the development server**
   ```bash
   npm start
   # or
   expo start
   ```

4. **Run on your preferred platform**
   ```bash
   # Web Browser
   npm run web
   
   # Android Emulator/Device
   npm run android
   
   # iOS Simulator/Device
   npm run ios
   ```

## 🎮 Usage

### Quick Start
1. Launch the app to see the animated welcome screen
2. Navigate to the Home screen with the latest news
3. Browse articles by selecting different categories
4. Tap any article to view details
5. Use the heart icon to save articles to favorites
6. Access favorites from the navigation buttons
7. Create custom articles using the "My News" section

### Key Features in Action

**Filtering Articles:**
- Tap category buttons at the top to filter articles
- "All" category shows all available articles

**Managing Favorites:**
- Tap the heart icon on any article to save it
- View all favorites in the Favorites screen
- Remove favorites by tapping the heart icon again

**Creating Custom Articles:**
- Navigate to "My News" from the Home screen
- Tap "Add New Article" to create content
- Fill in title, image URL, and description
- Edit or delete your articles anytime

## 📁 Project Structure

```
NewsArticles/
├── src/
│   ├── components/          # Reusable UI components
│   │   ├── articles.js      # Article grid and cards
│   │   └── categories.js    # Category filter bar
│   ├── screens/            # App screens
│   │   ├── WelcomeScreen.js # Animated welcome screen
│   │   ├── HomeScreen.js    # Main news feed
│   │   ├── ArticleDetailScreen.js # Article details view
│   │   ├── FavoriteScreen.js # Saved articles list
│   │   ├── MyArticlesScreen.js # User's custom articles
│   │   ├── CustomNewsScreen.js # Custom article viewer
│   │   └── NewsFormScreen.js  # Article creation/editing form
│   ├── navigation/         # Navigation setup
│   │   └── index.js       # Stack navigator configuration
│   ├── redux/             # State management
│   │   ├── store.js       # Redux store configuration
│   │   └── favoritesSlice.js # Favorites reducer and actions
│   └── utils/             # Utilities
│       └── data.js        # Sample articles and categories data
├── assets/                # Images and icons
├── App.js                 # Main app component
├── app.json              # Expo configuration
├── package.json          # Dependencies
└── README.md             # This file
```

## 🔧 Development

### Available Scripts

```bash
# Start development server
npm start

# Run on web browser
npm run web

# Run on Android
npm run android

# Run on iOS
npm run ios

# Build for production (Android)
npm run build:android

# Build for production (iOS)
npm run build:ios

# Clear cache and restart
expo start --clear
```

### Key Development Files

- **`App.js`**: Main application wrapper with Redux Provider
- **`src/navigation/index.js`**: Navigation stack configuration
- **`src/redux/store.js`**: Redux store setup with middleware
- **`src/redux/favoritesSlice.js`**: Favorites state management logic

## 📱 Building for Production

### Android APK
```bash
# Install EAS CLI
npm install -g eas-cli

# Login to Expo
eas login

# Configure project
eas build:configure

# Build APK
eas build -p android --profile preview
```

### iOS IPA
```bash
# Build for iOS
eas build -p ios --profile preview
```

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. **Fork the repository**
2. **Create a feature branch**
   ```bash
   git checkout -b feature/amazing-feature
   ```
3. **Commit your changes**
   ```bash
   git commit -m 'Add amazing feature'
   ```
4. **Push to the branch**
   ```bash
   git push origin feature/amazing-feature
   ```
5. **Open a Pull Request**

### Development Guidelines
- Follow existing code style and structure
- Add comments for complex logic
- Test on multiple platforms if possible
- Update documentation as needed

## 🐛 Troubleshooting

### Common Issues

**1. Metro Bundler won't start:**
```bash
expo start --clear
# or
rm -rf node_modules && npm install
```

**2. Android/iOS build failures:**
- Ensure you have the required SDKs installed
- Check Expo documentation for platform-specific requirements

**3. Navigation errors:**
- Verify all screen names match in navigation configuration
- Check that components are properly exported

**4. Redux state not updating:**
- Ensure you're using the correct action creators
- Check reducer logic in favoritesSlice.js

### Getting Help
- Check the [Expo documentation](https://docs.expo.dev/)
- Search existing [GitHub issues](../../issues)
- Create a new issue with detailed error information

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- **React Native Community** for the amazing framework
- **Expo Team** for the excellent development tools
- **Redux Team** for powerful state management
- **Contributors** who help improve this project

## 👥 Authors

- **Ewuzie Azuka Okwuchukwu** - [@ewuwise](https://github.com/ewuwise)

## 📞 Support  +2349160006401

For support, questions, or feedback:
- 📧 Email: ewuzieazuka001@gmail.com
- 🐛 [Create an Issue](../../issues/new)
- 💬 Discussions: Coming soon

---

<div align="center">

### ⭐ Star this repo if you find it helpful!

[![Star History Chart](https://api.star-history.com/svg?repos=ewuwise/NewsArticles&type=Date)](https://star-history.com/#ewuwise/NewsArticles&Date)

**Built with ❤️ using React Native & Expo**

</div>
