# Demo of react-native-static-server

This example project demonstrates the use of [`react-native-static-server`](https://github.com/birdofpreyru/react-native-static-server) on Android. 

The work was done on Ubuntu 22 with a physical mobile device.

These were the steps taken to get it working:

## Start with default React Native 0.73.7 project

This project was initialized using the standard React Native command line tools.

```
npx react-native@0.73.7 init ReactNativeStaticServer --version 0.73.7
```

## Copy App.tsx to project

[App.tsx is copied from react-native-static-server project's example](https://raw.githubusercontent.com/birdofpreyru/react-native-static-server/master/example/src/App.tsx).

## Update android/build.gradle minSdkVersion

Package `react-native-static-server` requires minSdkVersion to be 28, so I updated `android/build.gradle` accordingly.

## npm install required packages

Finally, npm was used to install required packages:

```
npm i '@dr.pogodin/react-native-static-server'
npm i react-native-webview
npm i @dr.pogodin/react-native-fs
```

## Run

In one terminal window, run `npm start`. In a second terminal, run `npm run android`.