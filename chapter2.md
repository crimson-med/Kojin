# The Principle

## Firebase

**Firebase** is a google module to help with mobile development. It focuses on bringing Authentification, Notifications, Stats to mobile development easily.

For our part we will take a look at the **Firebase Notifications** which actually use whats called **Firebase Cloud Messaging.**

This is the module of the project that will let us send notification to our users very easily.

## The Exploit

In React Native the goal is when an App is in background the Javascript is actually paused and hense nothing really runs.

However for any reasons possible maybe you would like that when a Notification is received some Javascript code is ran or called.

This is a easy way to deliver a command without having your App scanning an API Endpoint every X seconds for a new command.

This resided in the simplicity of this code.

## React Native

For the React Native App we will be using only:

 - DeviceEmitters
 - Firebase Cloud Messaging

 I will be using this package to handle the FCM:

     npm install react-native-fcm

This package only includes the FCM part and no Authentification or the rest of the options of Firebase hence it is more lightweight.

## Visual Representation

Here is a example of how the system works:

//image
