# Foreword

Before starting the coding here please make sure you have followed the [Environment Setup](/chapter1.md) and that you can run the default app with the `react-native-fcm` integration.

# App.js

First inside the App class we will add a constructor. This will let us save the fcm token this can be useful in the future if you want to send a notification to a single user. We will come back to this later.

```js
constructor(props) {
    super(props);
    this.state = {
        fcm_token: ""
    };
}
```

We will now work with componentWillMount\(\) to initialize the settings.

```js
componentWillMount() {
  FCM.requestPermissions();
  FCM.getFCMToken().then(token => {
    this.setState({fcm_token:token});
    //update your fcm token on server.
  }).catch((el) => {console.error(el)});
}
```



