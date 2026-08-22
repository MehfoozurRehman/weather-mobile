# Weather Forecast Mobile App

A cross-platform React Native mobile application for global real-time weather forecasts, hourly conditions, and multi-city weather tracking.

## Overview

`weather-mobile` delivers comprehensive atmospheric forecasts, temperature curves, humidity/wind metrics, and multi-tab location switching with smooth gesture navigation.

## Tech Stack

- **Framework**: React Native (v0.82) / React 17
- **Navigation**: React Navigation (Bottom Tabs, Material Top Tabs, Drawer, Stack)
- **Animations & Gestures**: `react-native-reanimated`, `react-native-gesture-handler`, `react-native-tab-view`

## Prerequisites

- Node.js (v16 or v18 recommended)
- Android Studio / Xcode configured with Android SDK / CocoaPods
- Package manager (`pnpm` or `npm`)

## Getting Started

1. **Install dependencies**:
   ```bash
   pnpm install
   # or
   npm install
   ```

2. **Install iOS Pods** (macOS only):
   ```bash
   cd ios && pod install && cd ..
   ```

3. **Start Metro Bundler**:
   ```bash
   npm start
   ```

4. **Launch on Device / Simulator**:
   - Run on Android: `npm run android`
   - Run on iOS: `npm run ios`

## Available Scripts

- `npm start` - Launches the React Native Metro bundler.
- `npm run android` - Compiles and runs the Android application.
- `npm run ios` - Compiles and runs the iOS application.
- `npm test` - Runs Jest test suites.
- `npm run lint` - Runs ESLint code quality checks.

## Author

Created by [Mehfooz-ur-Rehman](https://github.com/MehfoozurRehman).
