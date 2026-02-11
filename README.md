# RNFLAndroidDemo

A React Native Android demo app with Fastlane and CI/CD via GitHub Actions.

## Build

```bash
npm install
cd android && bundle install && bundle exec fastlane android build
```

The debug APK will be at `android/app/build/outputs/apk/debug/app-debug.apk`.

## CI/CD

The GitHub Actions workflow builds the debug APK using Fastlane and uploads it to AutoDevice on every push to `main`.

### Required Secrets

- `AUTODEVICE_API_KEY` — API key for AutoDevice
