# ConvoKit Android Maven repository

Public release artifacts and metadata for ConvoKit's unauthenticated Android
Maven feed. Cloudflare Pages publishes this repository at
<https://maven.convokit.app> whenever `main` changes.

Add the repository in `settings.gradle.kts`:

```kotlin
dependencyResolutionManagement {
    repositories {
        google()
        mavenCentral()
        maven("https://maven.convokit.app/")
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

The implementation repository is private. This repository contains compiled
release artifacts and Maven metadata only.
