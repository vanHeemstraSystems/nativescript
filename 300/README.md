# 300 - Building Our Application

Based on "NativeScript Tutorial for Beginners - Build iOS, Android and Web Apps with NativeScript" at https://www.youtube.com/watch?v=8Q8OtgL3Fuo

## Create a new App

Run the following command from containers/app directory:

```
$ tns create HelloWorld --template nativescript-template-tutorial
```

If you receive an error like "No matching version found for nativescript-template-tutorial" just leave out the template option:

```
$ tns create HelloWorld
```

Without the template, you will be provided with alist of styles to choose from:

```
# Let’s create a NativeScript app!

Answer the following questions to help us build the right app for you. (Note: you
can skip this prompt next time using the --template option, or the --ng, --react, --vue, --svelte, --ts, or --js flags.)

? First, which style of NativeScript project would you like to use: › - Use arrow-keys. Return to submit.
❯   Angular - Learn more at https://nativescript.org/angular
    React
    Vue.js
    Svelte
    Plain TypeScript
    Plain JavaScript
```

This time we will choose **Svelte**. Point at it with your Up/Down keys and hit ENTER when on Svelte.

You will be informed as follows:

```
[@nativescript/webpack] Initialized config.
Project HelloWorld was successfully created.

Now you can navigate to your project with cd HelloWorld and then:

Run the project on multiple devices:

  $ ns run ios
  $ ns run android

Debug the project with Chrome DevTools:

  $ ns debug ios
  $ ns debug android

For more options consult the docs or run ns --help
```

Go into the new project directory:

```
$ cd HelloWorld
```

At any time you can run the ```tns --help``` command to open the NativeScript CLI documentation in your terminal.

Also, check the version of your NativeScript CLI with:

```
tns --version
8.6.1
✔ Up to date.
```

## Running Apps

In NativeScript CLI you run the ```ns run``` command to run your apps on iOS or Android. **NOTE**: In older versions of NativeScript the command was **tns**, nowadays it is **ns**, whilst **tns** is still supported.

Let's start with **Android**.

Run the following command to start the Android emulator:

```
$ ns run android
```

You may be prompted as:

```
✔ Javac is installed and is configured properly.
✔ The Java Development Kit (JDK) is installed and is configured properly.
✔ Local builds for iOS can be executed only on a macOS system. To build for iOS on a different operating system, you can use the NativeScript cloud infrastructure.
✖ The ANDROID_HOME environment variable is not set or it points to a non-existent directory. You will not be able to perform any build-related operations for Android. 
 To be able to perform Android build-related operations, set the `ANDROID_HOME` variable to point to the root of your Android SDK installation directory. 

✖ WARNING: adb from the Android SDK is not installed or is not configured properly.  
 For Android-related operations, the NativeScript CLI will use a built-in version of adb.
To avoid possible issues with the native Android emulator, Genymotion or connected
Android devices, verify that you have installed the latest Android SDK and
its dependencies as described in http://developer.android.com/sdk/index.html#Requirements 

✖ WARNING: The Android SDK is not installed or is not configured properly. 
 You will not be able to run your apps in the native emulator. To be able to run apps
in the native Android emulator, verify that you have installed the latest Android SDK 
and its dependencies as described in http://developer.android.com/sdk/index.html#Requirements 

✖ Cannot find a compatible Android SDK for compilation.
To be able to build for Android with your current android runtime, install one of the following supported Android SDK targets:
  android-17
  android-18
  android-19
  android-20
  android-21
  android-22
  android-23
  android-24
  android-25
  android-26
  android-27
  android-28
  android-29
  android-30
  android-31
  android-32
  android-33
Supported targets vary based on what android runtime you have installed. Currently your app uses @nativescript/android null 
 Run `$ sdkmanager` to manage your Android SDK versions. 

✖ No compatible version of the Android SDK Build-tools are installed on your system. You can install any version in the following range: '>=23 <=33'. 
 Install the required build-tools through Android Studio. In case you already have them installed, make sure the `ANDROID_HOME` environment variable is set correctly. 

Your environment is not configured properly and you will not be able to execute local builds.
Verify that your environment is configured according to the system requirements described at
https://docs.nativescript.org/setup/linux#setting-up-linux-for-android.
```

See "NativeScript Windows Setup - Step by Step" at https://www.youtube.com/watch?v=3O-rsAFw8J8 for preparing for Android.

Type ```CTRL + C``` to stop the Android emulator.

Let's for now continue with **iOS**.

Run the following command to start the iOS emulator:

**NOTE**: NativeScript uses **XCode** under the hood to build and run iOS Apps. And XCode is only available on MacOS. Therefore you can only run iOS Apps on MacOS.

```
$ ns run ios
```
 
If above command is run on a platform other than iOS (so not on a Mac), you will be prompted as follows:

```
Applications for platform iOS can not be built on this OS
```

If instead you want to make sure of an emulator to develop this application further, you can continue as follows:


```
$ ns preview
```

You will be presented with a QR code (in the GitPod Terminal window or the sidepanel), which you need to scan with your iOS device (iPhone or iPad, on which your previously installed the NativeScript preview App from the App Store).

You should now see the NativeScipt app on your iPhone or iPad, ready to monitor whilst developing further, as it will be synced.

MORE ...