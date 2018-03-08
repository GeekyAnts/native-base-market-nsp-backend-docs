# Deploy Api-Server, Mobile App in Local machine

####  Requirement
   
  * [npm](https://www.npmjs.com/) installed along with [node](https://nodejs.org/en/)
  * [MongoDB](https://www.mongodb.com/) 

#  Api server 

 
  
####  Installation Steps

Step1: Download the Native Startter pro app and extract it

Step2: Open terminal and Go to Full-apps folder where you have extracted, there you would find 3 modules api-server, mobile-app 

Step3: Goto api-server folder and install npm or yarn ```npm install``` or ```yarn```

Step4: Start the api server ```npm start``` now api-server is up and running

Step5:  Open an another terminal and enter ```mongod``` this would start mongo server 

 ####  Common issue of mongo server 

   unable to lock file: /data/db/mongod.lock resource temporarily unavailable. Is a mongod instance already running? , terminating, 
    You need to enter,  
    ```sudo killall -15 mongod```


# Mobile App
  
   #### Installation steps 

  <!-- Note: Before Starting Mobile app you need to seed the database follow Step1 of Admin Dasbhboard  -->

<!-- Steps: Initiate app for app folder  -->

  * cd NativeStarterPro-backend
  * Type ```npm i ```  
  * Type  npm start

  * If you would like to run app in android you need to connect the android phone  to a system or via android emulator, and type ```npm run android``` Make   sure you have configured the AVD before running the command,If you would like to run app in iPhone simulator (MacOS) run ```npm run iOS```

      Note : Make sure you have same network in the mobile  
