# Deploying code on Server

Deploying is a big part of the lives of most  developers . We don't have a release manager and there are no set weekly deploys. Developers and designers are responsible for shipping new stuff themselves as soon as it's ready. This means that deploying needs to be as smooth and safe a process as possible.

The best system we've found so far to provide this flexibility is to have people deploy branches. We have taken special care of to roll out repetitive work so if any new branch merges with master it automatically deploy itself.

We have taken special care that master remains stable and is always working with the latest for that we have two servers namily

Staging and Production .This means that master is always stable; a safe point that we can roll back to if there's a problem.By default staging server points to the Develop/Development branch of the code and production server points to master branch of the code.

### Deploying Libraries

There may be times when you want to make a library available to your team without making it public. This is best done by setting up a private repository. 

#### Static HTTP

The simplest kind of private repository is a web server pointed at a directory full of static files. You can use a`file:///`URL in your`:repositories`to deploy that way if the directory is local to the machine on which Leiningen is running.

#Setting up the NativeStarterPro-backend

## LOCAL SERVER
1.clone the repo from 
  ```
  http://gitstrap.com/strapmobile/NativeStarterPro-backend.git
  ```

2. goto project cloned repo.
3. git pull origin <branch-name>
4. In app directory open `./config/test.json`.Here you will find the configuration of host and port number
    ```
    {
    env: 'test',
    jwtSecret: '0a6b944d-d2fb-46fc-a85e-0295c986cd9f',
    db: 'mongodb://localhost/express-mongoose-es6-rest-api-test',
    port: 3000
    }
    ```
    you can edit the environment configuration variables here.
  -  edit  `~./bashrc` and add `export NODE_ENV=test`
  - run `npm start`

## STAGING OR PRODUCTION SERVER
### Step 1:
To access the server you can **SSH**:-
      Staging - `ssh messaging-app-backend@ded1.geekydev.com`
      Production - `ssh messaging-app-backend-staging@ded1.geekydev.com`

### Step 2:
Go inside the project directory `cd Sites/projects/NativeStarterPro-backend`  

1. For STAGING
    - git pull origin development
    -  in app directory open `./config/development.json`
    ```
    {
      env: 'development',
      jwtSecret: '0a6b944d-d2fb-46fc-a85e-0295c986cd9f',
      db: 'mongodb://localhost/express-mongoose-es6-rest-api-development',
      port: 3000
    }
    ```
  - edit  `~./bashrc` and add `export NODE_ENV=production`
  - git commit -am "YOUR MODIFICATION MESSAGE"
  - git push origin development
  - Restart the server:
    `node src/index.js`
    `forever list`
      - You will get an id of the app, from which you can
    `forever restart <ID>`

2. For PRODUCTION
    - git pull origin master
    -  in app directory open `./config/production.json`. This is where you will find the configuration settings.
        ```
        {
           env: 'production',
           jwtSecret: '0a6b944d-d2fb-46fc-a85e-0295c986cd9f',
           db: 'mongodb://localhost/nsp-node-production',
           port: 3030
        }

        ```
    - edit `~./bashrc` and add `export NODE_ENV=production`
    - git commit -am "YOUR MODIFICATION MESSAGE"
    - git push origin development
    - Restart the server:
      `node src/index.js`
      `forever list`
      - You will get an id of the app, from which you can
    `forever restart <ID>`


  


