# Configure Kotlin

## Kotlin plugin
1. Open Android Studio settings: `CMD` + `,`
2. Type `plugins` in search bar
3. Click on `Browse repositories`
4. Search and install `Kotlin` plugin from `CUSTOM LANGUAGES`
5. Restart Android Studio

## Add Kotlin to project
1. Open `Action and option` dialog box: `CMD` + `SHIFT` + `A`
2. Type `Configure Kotlin in Project`
3. Choose `Android with Kotlin`
4. Configure Kotlin for all modules
5. Click on `Sync Now`

## Add [Android Extensions](https://kotlinlang.org/docs/tutorials/android-plugin.html)
1. Open `app/build.gradle`
2. Apply plugin `kotlin-android-extensions`

When project synced go to [next step](03_ConvertJavaClassToKotlin.md)
