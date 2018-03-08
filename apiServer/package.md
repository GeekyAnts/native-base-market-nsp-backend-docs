# Packages Used

_package.json_

<pre class="line-numbers"><code class="language-json">
{
  "name": "native-starter-pro-back-end",
  "version": "8.0.0",
  "main": "index.js",
  "private": false,
  "scripts": {
    "start": "gulp serve",
    "build": "gulp",
    "lint": "gulp lint",
    "test": "gulp mocha",
    "commit": "git-cz",
    "report-coverage": "coveralls < ./coverage/lcov.info"
  },
  "dependencies": {
    "bcrypt": "^1.0.3",
    "bluebird": "^3.5.1",
    "body-parser": "^1.18.2",
    "compression": "^1.7.1",
    "cookie-parser": "^1.4.3",
    "cors": "^2.8.4",
    "debug": "^3.1.0",
    "express": "4.16.2",
    "express-jwt": "5.3.0",
    "express-validation": "1.0.2",
    "express-winston": "^2.4.0",
    "helmet": "3.9.0",
    "http-status": "^1.0.1",
    "joi": "13.0.2",
    "jsonwebtoken": "8.1.0",
    "method-override": "^2.3.10",
    "mongoose": "^4.13.5",
    "morgan": "1.9.0",
    "path": "^0.12.7",
    "winston": "^2.4.0"
  },
  "devDependencies": {
    "babel-cli": "6.26.0",
    "babel-core": "^6.26.0",
    "babel-plugin-add-module-exports": "0.2.1",
    "babel-preset-es2015": "6.24.1",
    "babel-preset-stage-2": "6.24.1",
    "chai": "^4.1.2",
    "commitizen": "^2.9.6",
    "coveralls": "^3.0.0",
    "cz-conventional-changelog": "2.1.0",
    "del": "^3.0.0",
    "eslint": "^4.12.0",
    "eslint-config-airbnb": "16.1.0",
    "eslint-plugin-import": "^2.8.0",
    "ghooks": "^2.0.1",
    "gulp": "3.9.1",
    "gulp-babel": "7.0.0",
    "gulp-env": "^0.4.0",
    "gulp-eslint": "^4.0.0",
    "gulp-istanbul": "1.1.2",
    "gulp-load-plugins": "^1.5.0",
    "gulp-mocha": "^4.3.1",
    "gulp-newer": "^1.3.0",
    "gulp-nodemon": "^2.2.1",
    "gulp-plumber": "^1.1.0",
    "gulp-sourcemaps": "^2.6.1",
    "gulp-util": "^3.0.8",
    "isparta": "4.0.0",
    "jsonwebtoken": "8.1.0",
    "mocha": "4.0.1",
    "passport": "^0.3.2",
    "passport-jwt": "^2.1.0",
    "run-sequence": "^2.2.0",
    "supertest": "^3.0.0",
    "supertest-as-promised": "4.0.2",
    "validate-commit-msg": "^2.14.0"
  },
  "config": {
    "ghooks": {
      "pre-commit": "npm run lint && npm test",
      "commit-msg": "validate-commit-msg"
    },
    "commitizen": {
      "path": "./node_modules/cz-conventional-changelog"
    }
  },
  "babel": {
    "presets": [
      "es2015",
      "stage-2"
    ],
    "plugins": [
      "add-module-exports"
    ]
  }
}
</code></pre>
