# Android WebRTC Library

<img src="https://www.gstatic.com/devrel-devsite/prod/v70c5e166a48b2c4e0a0d27f0b12c8c47a28a215b513b1100ea89abd1a9e8a095/webrtc/images/lockup.svg" alt="webrtc.org" width="400">

## Integrate Into Android Project
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

Add dependency to your app module (such as app/build.gradle), latest availabe stable version in this repo is **M83**:
```xml
dependencies {
    implementation 'com.aar.app:google-webrtc:M83'
}
```

## Description

This is precompiled google webrtc library for android, [https://webrtc.org/](https://webrtc.org/).
[repo branch](https://github.com/abdularis/libwebrtc-android/tree/repo)

read [this article](https://medium.com/@abdularis/how-to-compile-native-webrtc-from-source-for-android-d0bac8e4c933) on how to compile webrtc for android.

Use maven to add .aar library into the existing maven repository using:
```
mvn install:install-file -Dfile=./google-webrtc-M74.aar -DgroupId=com.aar.app -DartifactId=google-webrtc -Dversion=M74 -Dpackaging=aar -DlocalRepositoryPath=./libwebrtc-android -DcreateChecksum=true
```
