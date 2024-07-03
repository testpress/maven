# Getting Started
This SDK enables you to securely stream DRM-protected videos through your Android app.

### Add TPStreams maven repo to app module's `build.gradle`

```
repositories {
    maven {
        url "https://github.com/testpress/maven/raw/main/repo"
    }
}
```

### Add player dependency to app project `build.gradle`

```
// Use the latest version available for integration.

// To integrate the TPStreams player
implementation 'com.tpstreams.player:player:3.0.20'

// If you're already using Exo Player in youe project, you can still integrate TPStreams Player with below implimentation.

// To integrate the TPStreams player
implementation 'com.tpstreams.player:player:2.0.20'
```

### Enable Java 8 support

You also need to ensure Java 8 support is enabled by adding the following block to each of your app module's `build.gradle` file inside the `android` block:

```
compileOptions {
    sourceCompatibility JavaVersion.VERSION_1_8
    targetCompatibility JavaVersion.VERSION_1_8
}
```

### Using ProGuard

```
-keep class com.tpstream.player.** { *; }
```

## Documentation
* The [TPStreams] developer guides offer a wealth of information.

[TPStreams]: https://developer.tpstreams.com/docs/mobile-sdk/android-native-sdk/getting-started