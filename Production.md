# Deploy Api-Server, Mobile App in Production


# Api server

#### Installation steps
Clone the app 

Step1: Go to api-server folder     
* Enter ``` npm i ```

Step2:  Enter ```npm run build```

Step3:  Export node environment by ```export NODE_ENV=production``` Do check if it is set by ```echo $NODE_ENV``` it Prompts as production.

Step4: Run forever now enter ```forever start dist/index.js``` Check if forever is running by entering ```forever list```

#### Common issues npm ERR! bcrypt

You need to enter ```npm install --save bcrypt-nodejs && npm uninstall --save bcrypt```




# Mobile App(Rider/Driver)
 
 Make sure you have an expo account .
 

  i) To publish it on Expo and get the expo link 
  
  Go to the respective mobileApp folder (RiderApp/DRiverApp) and
  run  ```exp publish```

  ii) [To build standalone app ](https://docs.expo.io/versions/v16.0.0/guides/building-standalone-apps.html#content)


  a) [Configure app.json](https://docs.expo.io/versions/v16.0.0/guides/building-standalone-apps.html#2-configure-expjson)

  You need to configure rather update the default app.json and add the various values that you will need to build standlone app(apk & ipa).

  b) [Start the build](https://docs.expo.io/versions/v16.0.0/guides/building-standalone-apps.html#3-start-the-build)

 Run ```exp start``` in your app directory to boot up the Expo packager. This is necessary because during the build process your app will be republished to ensure it is the latest version.

 i) If you choose to build for Android

 Once the app has started, run ```exp build:android```

 ii) If you choose to build for iOS

 Once the app has started, run ```exp build:ios```

 c) Wait for it to finish building

  This will take a few minutes, you can check up on it by running ```exp build:status```. When it’s done, you’ll see the url of a .apk (Android) or .ipa (iOS) file — this is your app.




