# Tab Activity Template
-
Tab Activity template for android studio

![Screenshoot app](https://drive.google.com/open?id=1i4WyIz9-3YOH6FjjcfgY1Oq9R0_ZA8I4)

## Getting Started
-
These instructions will get you a copy of the project up and running on your local machine.

### Prerequisites
-
- Before you begin to the installation, you need to install * [Android Studio](https://developer.android.com/studio/).
- in your android studio project you must add this in your `build.gradle(app)` depedencies
```
dependencies {
  ...
  implementation 'com.android.support:design:28.0.0'
  ...
}
```
- and implement dataBinding in your `build.gradle(app)` android
```
android {
  ...
  dataBinding {
        enabled true
  }
}
```

### Installing
-
- Clone or download this repo
- Copy folder TabActivityTemplate to 
for windows user:
```
{ANDROID_STUDIO_LOCATION}/plugins/android/lib/templates/activities/
```
for mac user:
```
/Applications/Android Studio.app/Contents/plugins/android/lib/templates/activities/
```
- open Android Studio (if you already opened android studio, restart it)
- right click on a package that you want to create the template in and select it from the “New” menu, as below:
![Create the template](https://drive.google.com/open?id=1avAVzy1jRqAmDzpU_FmX-_9FCfleU9g-)
- You will then be prompted to fill in the variables see the example below:
![Fill in the variable template](https://drive.google.com/open?id=1cpCaN9zgyj1rvpks6DlFR7I1hXqv0QEO)
- You will see some error code, that's because you must `import` some code before you can continue.
- if the error has gone, you must add this in your `androidManifest.xml`
if this is your first activity, than use this code
```
<manifest ...>
    <application ...>
        
        <activity android:name="{name of your activity}">
            <intent-filter>
                <action android:name="android.intent.action.MAIN" />

                <category android:name="android.intent.category.LAUNCHER" />
            </intent-filter>
        </activity>
        
    </application>
</manifest>
```
but if there is another activity existed use this code
```
<manifest ...>
    <application ...>
        
        <activity android:name="{name of your activity}"></activity>
        
    </application>
</manifest>
```
- You can modify the code as you like.

## Running the app
-
to run your app. you can use your android device or use the emulator.
just click this icon ![Run icon](https://drive.google.com/open?id=1l7gTWW1O6YD8DDQI0mqAY_eRv2ksRGwl)

![Screenshoot app](https://drive.google.com/open?id=1i4WyIz9-3YOH6FjjcfgY1Oq9R0_ZA8I4)

## Authors

* **Anang Kurniawan** - *Initial work* - [AnangKur](https://github.com/anangkur)

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

* Hat tip to anyone whose code was used
* Inspiration
* etc