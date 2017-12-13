# Building the exploit

## Firebase

First lets create a Firebase account here:

**link**

Then configure an API Key if it's not done by default.

## React Native

### Workspace

For the React Native App we will be editing only **App.js** as that's is the module that wraps the whole application. If you root module isn't called App.js you can always rename of just edit yours.

First we need to handle hooking the Notification Receivers to the proper functions of our module.

We will be working with **ComponentWillMount()**

### Handling DeviceEmitters

For thos who don't know DeviceEmitters are a very powerful tool that can be used in React Native.

You Hook an module in it's ComponentWillMount() function and then in any other module Parent or Child you can call it and the DeviceEmitters component will call on the function you defined.

This can be used for instance if a user uses points on a specific page of your app you can call the DeviceEmitters to update the points already rendered.
