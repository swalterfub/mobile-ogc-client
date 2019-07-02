# Apache Cordova

## Android

### Prerequisites

- [Android SDK Tools](https://developer.android.com/studio/index.html)

- [Gradle](https://gradle.org/install/)

- [Direct dependencies for Cordova](https://cordova.apache.org/docs/en/latest/guide/platforms/android/index.html)
  ```
  sdkmanager "build-tools;29.0.0"
  sdkmanager "extras;android;m2repository"
  sdkmanager platform-tools
  ```
### Android Emulator

- [Set up android emulator](https://cordova.apache.org/docs/en/latest/guide/platforms/android/index.html#setting-up-an-emulator)
  ```
  sdkmanager "system-images;android-29;google_apis;x86_64"
  sdkmanager emulator
  avdmanager list
  avdmanager create avd -d 17 -n pixel -k "system-images;android-29;google_apis;x86_64"
  emulator -list-avds
  emulator @pixel
  ```

### Cordova

- [Install cordova and create HalloWorld](
  ```
  npm install -g cordova
  cordova create hello com.example.hello HelloWorld
- Adapt HelloWorld example
  ```
  cd hello
  vi www/index.html
  (paste code from Carlos)
  ```
- Run Cordova in the emulator
  ```
  cordova run android
  ```
  
