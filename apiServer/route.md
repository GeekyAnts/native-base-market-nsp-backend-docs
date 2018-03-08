## Routes - api/auth/login

##### Method: POST {#method-post}

Contains route which gets the email and password  from user .It search for the entry in database .If it exists then it returns a JWT along with user Object to user. These functionalities are included in login  route :-

#### login\(\) {#otpgenerate}

1. **Description:**
    It takes the email and password from the user. Search the database if the same data exists . It return a JWT Token back to user .
2. **Parameters:**  
     It takes two parameters ie. user Email and Password .
3. **Response:**  
  
```
       {

         "success": true,

         "message": "user created successfully",

         "data": {

           "jwtAccessToken": "JWT eyJhbGciOiJIUzI1NiIsI...",

           "user": {

             "\_\_v": 0,

             "email": "user@gmail.com",

             "password": "$2a$10$6U3AOzzdBbPH6a3kqA6.feei6GgvPSURkVHNdL13QhPFmnZVVTgnm",

             "phoneNo": "9191919191",

             "\_id": "57e272c7268e9103947bc472",

             "jwtAccessToken": null,

             "createdAt": "2016-09-21T11:45:11.898Z"

           }

         }

       }
```

## Routes - api/auth/logout

##### Method: GET {#method-post}

Contains route which gets the email and password  from user .It search for the entry in database .If it exists then it returns a JWT along with user Object to user. These functionalities are included in login  route :-

#### logout\(\) {#otpgenerate}

1. **Description:**
    It takes the  JWT Token from logined user .
2. **Parameters:  **
     It takes JWT Token from the user .
3. **Response:**

```
    {

   "success": true,

   "message": "user logout successfully"

   }  
 ```

## Routes - api/users/register

##### Method: POST {#method-post}

Contains route which gets the email and password  from user .It creates a new entry in database .If it exists then it returns a failed response to  user. These functionalities are included in register  route :-

#### create\(\) {#otpgenerate}

1. **Description:**
    It takes the email and password from the user. s . It return a JWT Token back to user .
2. **Parameters:**  
     It takes two parameters ie. user Email and Password .
3. **Response:**  
   ```

       {

         "success": true,

         "message": "user created successfully",

         "data": {

           "jwtAccessToken": "JWT eyJhbG...",

           "user": {

             "\_\_v": 0,

             "email": "user@gmail.com",

             "password": "$2a$10$6U3AOzzdBbPH6a3kqA6.feei6GgvPSURkVHNdL13QhPFmnZVVTgnm",

             "\_id": "57e272c7268e9103947bc472",

             "jwtAccessToken": null,

             "createdAt": "2016-09-21T11:45:11.898Z"

           }

         }

       }

     ```

## Routes - api/users/

##### Method: GET {#method-post}

Contains route which gets the detail of  all users .It returns complete user Object to user. These functionalities are included in user  route :-

#### get\(\) {#otpgenerate}

1. **Description:**
    It  find the details of the all the user that exist in database .
2. **Parameters:  **
     It takes JWT Token from the user .
3. **Response:**

```
   {

   "success": true,

   "message": "User found",

   "data": {

    "user": {

      "\_id": "57f7a4a94780025e27f8349b",

      "email": "user@gmail.com",

      "\_\_v": 0,

      "jwtAccessToken": null,

      "createdAt": "2016-10-07T13:35:37.378Z"

    }

   }

 }
 ```

## Routes - api/users/:userId

#### get\(\) {#otpgenerate}

1. **Description:**
    It takes the  userId from the user and find out the details corresponding to that userId.
2. **Parameters:  **
     It takes JWT Token from the user .

#### put\(\) {#otpgenerate}

1. **Description:**
    It takes the  userId from the user and find out the details corresponding to that userId.and update the details that is passed along with the userId.
2. **Parameters:  **
     It takes JWT Token from the user .along with the details user need to update .mainly Email or Password .

#### delete\(\) {#otpgenerate}

1. **Description:**
    It takes the  userId from the user and find out the details corresponding to that userId.and delete that userObject from the database .
2. **Parameters:  **
     It takes JWT Token from the user .



