# Ionic mobile apps

To run download the repo and run
```
ionic serve
```

  
# How was it implemented?

### Camera plugin
```
npm install --save @ionic-native/camera@beta   
ionic cordova plugin add cordova-plugin-camera
ionic cordova platform add ios
ionic cordova platform add android 
```

### SQL storage
```
ionic g service services/Photo
ionic cordova plugin add cordova-sqlite-storage
npm install --save @ionic/storage
```

### Deprecated stuff v3 -> v4
<ion-nav>

https://ionicframework.com/docs/developer-resources/guides/first-app-v4/intro