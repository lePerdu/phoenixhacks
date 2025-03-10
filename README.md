# Phoenix Hacks
This is the official repository for the Florida Polytechnic Hackathon Application
scheduled for January 2020

![Image of Bootscreen](https://github.com/jongan69/phoenixhacks/blob/master/src/img/2.gif?raw=true)

This is a mobile application built using react native on Mac OS, currently in development

In order to get the application working on your local device

## Prerequisites / Requirements
This application will require you to have the following wokring and installed

Currently runninng on
Node: v12.11.0
Expo: 35.0.0

Depending on the mobile development enviornement you are running, These are the steps you would take

## Using Expo

1. Install the Expo app from the app store (both IOS and Android)
2. `npm install`
3. `npm start`
4. Scan the QR code from the Expo CLI or web app using the Expo app


## MacOS (iOS or Andoroid)

For MacOS you must have Xcode and Android studio installed with command line tools, and a few other things

1. You can install Xcode from the App store and android studio from: https://developer.android.com/studio
2. Run xcode-select --install
3. brew install yarn
4. brew install node
5. brew install watchman
6. brew tap AdoptOpenJDK/openjdk
7. brew cask install adoptopenjdk8

Once these are installed, you can git pull the repository using these commands:

1. git clone https://github.com/jongan69/phoenixhacks.git
2. cd phoenixhacks
3. cd ios
4. pod install

Once pods install completes, you can
1. cd ..
2. npm install or yarn install , both work but perferably yarn

To run on iOS:
react-native run-ios

To run on Android (follow the android studio portion below for andorid to build properly):
react-native run-android

If setup properly, the metro bundler should build the app and the app will install on the virtual device


## Windows ( Andorid Only ) ( Untested since July )

In order to get the android working on windows, you should have the following:

Chocolately:
https://chocolatey.org

Android Studio:
https://developer.android.com/studio

Once you have this you should be able to get the following:
Java SE Development Kit (JDK)
Python 2 (run the following)

To do so run these commands:
1. choco install -y nodejs.install python2 jdk8
2. npm install -g react-native-cli
3. git clone https://github.com/jongan69/phoenixhacks.git

Assuming these steps went smoothly you will need to setup android studio:

Android Studio installs the latest Android SDK by default. Building a React Native app with native code, however, requires the Android 9 (Pie) SDK in particular. Additional Android SDKs can be installed through the SDK Manager in Android Studio.

The SDK Manager can be accessed from the "Welcome to Android Studio" screen. Click on "Configure", then select "SDK Manager".

![Image of Android Studio](https://facebook.github.io/react-native/docs/assets/GettingStartedAndroidStudioWelcomeWindows.png)

The SDK Manager can also be found within the Android Studio "Preferences" dialog,
under Appearance & Behavior → System Settings → Android SDK.
Select the "SDK Platforms" tab from within the SDK Manager, then check the box next to "Show Package Details" in the bottom right corner. Look for and expand the Android 9 (Pie) entry, then make sure the following items are checked:

Android SDK Platform 28
Intel x86 Atom_64 System Image or Google APIs Intel x86 Atom System Image
Next, select the "SDK Tools" tab and check the box next to "Show Package Details" here as well.
Look for and expand the "Android SDK Build-Tools" entry, then make sure that 28.0.3 is selected.

Finally, click "Apply" to download and install the Android SDK and related build tools.

Configure the ANDROID_HOME environment variable

The React Native tools require some environment variables to be set up in order to build apps with native code.

Open the System pane under System and Security in the Windows Control Panel, then click on Change settings....
Open the Advanced tab and click on Environment Variables....
Click on New...
to create a new ANDROID_HOME user variable that points to the path to your Android SDK.

The SDK is installed, by default, at the following location:

c:\Users\YOUR_USERNAME\AppData\Local\Android\Sdk

You can find the actual location of the SDK in the Android Studio "Preferences" dialog,
under Appearance & Behavior → System Settings → Android SDK.

Open a new Command Prompt window to ensure the new environment variable is loaded before proceeding to the next step.

4. Add platform-tools to Path

1. Open the System pane under System and Security in the Windows Control Panel, then click on Change settings....
2. Open the Advanced tab and click on Environment Variables....
3. Select the Path variable, then click Edit.
4. Click New and add the path to platform-tools to the list.

The default location for this folder is:

c:\Users\YOUR_USERNAME\AppData\Local\Android\Sdk\platform-tools


Once youre here

Open up an android virtual device and in command line:

1. cd phoenixhacks
2. npm install / yarn install
3. react-native run-android

The metro bundler should open and install the app on the virtualdevice


## Refrence these links for help
1. React native : https://facebook.github.io/react-native/docs/getting-started
2. Chocolaty: https://chocolatey.org
3. Cocoa pods: https://guides.cocoapods.org/using/getting-started.html
