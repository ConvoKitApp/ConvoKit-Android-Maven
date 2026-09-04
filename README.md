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

Add the core SDK and, optionally, the Jetpack Compose UI package in the
application module:

```kotlin
dependencies {
    implementation("app.convokit:convokit-android:0.1.0")
    implementation("app.convokit:convokit-android-ui:0.1.0")
}
```

See the [Android SDK documentation](https://convokit.app/docs/android-sdk) and
[public SDK example application](https://github.com/ConvoKitApp/ConvoKit-Android-SDK-Examples),
or the [Android UI documentation](https://convokit.app/docs/android-ui) and
[public UI examples](https://github.com/ConvoKitApp/ConvoKit-Android-UI-Examples).

The implementation repository is private. This repository contains compiled
release artifacts and Maven metadata only.
