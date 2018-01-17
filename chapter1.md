# Environment Setup

## Installing React Native

Through **npm** install react native using this command.

```
npm install -g react-native-cli
```

## Installing Android Studio

To install Android Studio just follow this link:

> [https://developer.android.com/studio/install.html](https://developer.android.com/studio/install.html)

## Initializing our first App

Simply use this command in the desired folder.

```
react-native init kojinExample
```

## Testing the App

First open Android Studio Open the **AVD Manager**

Create a new Virtual Device or use one of your owns.

For my part I use:

> Nexus 5X API 27

Once your emulator started you can simply run the command:

```
react-native run-android
```

If you want to use IOS Simulator you can simply run the command:

```
react-native run-ios
```

## Configuring Firebase

For this project we will use the React Native Firebase module developed by **evollu**.

To install the package:

```
npm install react-native-fcm --save
```

Then run the linking command:

```
react-native link react-native-fcm
```

Then just follow the steps described in the **Readme.md**. We will follow the Android configuration \([Introduction](/README.md)\)

[https://github.com/evollu/react-native-fcm\#configure-firebase-console](https://github.com/evollu/react-native-fcm#configure-firebase-console)

