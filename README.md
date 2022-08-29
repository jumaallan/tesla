# Tesla

Tesla App Clone built in Kotlin, using Compose. The project was initially designed by [Clinton, using Flutter](https://twitter.com/KChienja/status/1563932565442109442), with this [figma design](<https://www.figma.com/file/YZpVpudFO7BQfT8fuw8RiJ/Dark-Neumorphism-UI-Tesla-app-(Community)>)

We are keeping this repo as a single module since we are building out the UI only. Might modularize if necessary, but not now :smile:

## Dependencies

1. [Versions Catalog](https://docs.gradle.org/current/userguide/platforms.html#sub:version-catalog)
2. Jetpack Compose
3. Coil - For Image Loading and Caching
4. [Material3](https://m3.material.io/libraries/mdc-android/getting-started)
5. Hilt

### Versions Catalog

To add a dependency, navigate to **gradle/libs.versions.toml** file, which has all the dependencies for the project. This file has the following sections:

[versions] is used to declare the version numbers that will be referenced later by plugins and libraries.

[libraries] Define the libraries that will be later accessed in our Gradle files.

[bundles] Are used to define a set of dependencies. For this, we have `compose` and `hilt` as examples.

[plugins] Used to define plugins.

You need to add your dependency version in [versions]. This is unnecessary if you are not sharing the version across different dependencies. After defining the version, add your library in the [libraries] section as:

```toml
android-hilt = "com.google.dagger:hilt-android:2.42"
```

If you have already defined the version in [versions], you define it as:

```toml
android-hilt = { module = "com.google.dagger:hilt-android", version.ref = "hilt" }
```

## Designs

This is the link to the app designs:  
[Figma App Design](https://t.co/5tTiNQueMv)
