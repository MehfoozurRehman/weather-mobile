# Weather Forecast Mobile App

A React Native app shell for a weather forecast app. Navigation, gesture and animation libraries are installed, but the screen is still the React Native starter template, so no forecast data is shown yet.

## The problem

Checking the forecast on a phone should take one tap and show the outlook at a glance. This repo is the mobile foundation for that: a project that builds for Android and iOS, with a test and lint setup. The product screens and data layer are still to be written.

## What it does

What the code does today:

- Runs as a cross-platform React Native project with `android/` and `ios/` native projects and a root component in `App.js`.
- Renders the React Native template screen from `App.js` ("Step One", "See Your Changes", "Learn More").
- Has React Navigation packages installed (bottom tabs, drawer, stack and material top tabs), but none are wired into the app.
- Has gesture, animation and tab-view libraries installed (`react-native-gesture-handler`, `react-native-reanimated`, `react-native-tab-view`), with no source files using them yet.
- Includes a Jest test (`__tests__/App-test.js`) that renders the root component, plus ESLint and Prettier configuration.

## How it's built

- **Framework**: React Native 0.82, with React 17.0.2 pinned in `package.json`.
- **Navigation**: React Navigation 5 packages.
- **Tooling**: Jest 27 with the `react-native` preset, ESLint 7, Babel with `metro-react-native-babel-preset`.
- **Structure**: one root component (`App.js`) registered in `index.js`. There are no screens, services or data layer in the repo yet.

## Running it locally

Requires Node.js 16 or 18, plus the Android SDK and/or Xcode (with CocoaPods on macOS).

```bash
pnpm install   # or: npm install
cd ios && pod install && cd ..   # macOS only
npm start
```

In another terminal, run `npm run android` or `npm run ios`.

Other scripts: `npm test` (Jest) and `npm run lint` (ESLint).

## What I learned / what I'd do next

- The versions do not line up. React Native 0.82 is normally paired with React 19, but this project pins React 17, React Navigation 5, Reanimated 2 and Gesture Handler 1. Confirm the app builds and runs before adding features, and align the versions or pick a newer stack.
- The forecast features described in the earlier README (hourly conditions, temperature curves, multi-city tracking) are not in the code.
- There is no weather data source or API client yet. Choose a provider and add a thin client module.
- Replace the template screen and wire up the navigators that are already installed.
- The test only checks that the root component renders. Add tests for real screens as they arrive.

## Author

Created by [Mehfooz-ur-Rehman](https://github.com/MehfoozurRehman).
