# Expo Bet

A minimal Expo + React Native app template configured for Android Play publishing.

Features:
- Expo app scaffolded with TypeScript
- Google Play-ready `app.json`
- EAS build configuration for Android AAB output
- Ready for `paid app` configuration in Google Play Console

## Requirements
- Node.js 18+
- Expo CLI
- EAS CLI
- Google Play Developer account

## Install

```bash
npm install
```

## Run locally

```bash
npm start
```

## Build Android AAB

```bash
npm install -g eas-cli
npx eas login
eas build -p android --profile production
```

## Upload to Google Play

1. Create a new app in Google Play Console.
2. Set the app pricing to paid in the Play Console.
3. Upload the `.aab` from the EAS build.
4. Complete the store listing and submit for review.

Important:
- Google Play handles the price setting for a paid app.
- The app code does not automatically enforce a payment gate.
- To make a paid app, configure pricing in the Play Console and optionally use Play Billing if needed.

## Package name

Current package name:

```text
com.expobet.app
```

You can change it in `app.json` before publishing.
