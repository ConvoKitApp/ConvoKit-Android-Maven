# ConvoKit Android Maven repository

Public, unauthenticated Maven artifacts for the native ConvoKit Android SDK.

Add the repository in `settings.gradle.kts`:

```kotlin
dependencyResolutionManagement {
    repositories {
        google()
        mavenCentral()
        maven("https://convokitapp.github.io/ConvoKit-Android-Maven/")
    }
}
```

Add the SDK in the application module:

```kotlin
dependencies {
    implementation("app.convokit:convokit-android:0.1.0")
}
```

See the [Android SDK documentation](https://convokit.app/docs/android-sdk) and
[public example application](https://github.com/ConvoKitApp/ConvoKit-Android-SDK-Examples).

The implementation repository is private. This repository contains release
artifacts and Maven metadata only.
