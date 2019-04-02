# libwebrtc-android

This is precompiled google webrtc android library, [https://webrtc.org/](https://webrtc.org/)

## Usage
Add repository in the root gradle file:
```xml
...
allprojects {
    repositories {
        ...
        maven {
            url 'https://raw.github.com/abdularis/libwebrtc-android/repo/'
        }
    }
}
```

Add dependency to your app module (such as app/build.gradle), latest availabe stable version in this repo is M74:
```xml
dependencies {
    implementation 'com.aar.app:google-webrtc:M74'
}
```
