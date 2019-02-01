# Ionic mobile apps
Requirements
- Node.js
- cordova (npm install -g cordova)
- ionic   (npm install -g ionic)


######To run download the repo in the browser
```
npm install
ionic serve
```
######IOS
`ionic cordova platform add ios && ionic cordova build ios`

######Android
`ionic cordova run android`

######To run in lab environment for Android & IOS 
`npm i @ionic/lab@ && ionic lab`


#####Folder structure 
```
➜  myApp git:(master) ✗ tree -L 1
.
├── angular.json        ## Config for Ionic/Angular
├── config.xml          ## Used once the native project is built from the Ionic project
├── e2e                 ## Testing configurations
├── ionic.config.json
├── node_modules        ##  Downloaded dependencies defined in package.json 
├── package.json        ## Defines dependencies && plugins && packages
├── platforms
├── plugins             ## Cordova plugins
├── resources
├── src                 ## Code base
└── www                 ## Current build
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

### Login Screen
```
ionic g page public/login
ionic g page public/register
ionic g page members/dashboard
ionic g service services/authentication
ionic g service services/authGuard
ng generate module members/member-routing --flat
``` 

### Deprecated stuff v3 -> v4
<ion-nav>

https://ionicframework.com/docs/developer-resources/guides/first-app-v4/intro
