# Packages Used

_package.json_

<pre class="line-numbers"><code class="language-json">
{
  "name": "nativestarterpro",
  "version": "7.0.0",
  "private": true,
  "dependencies": {
    "expo": "^15.1.0",
    "react": "~15.4.0",
    "react-native": "0.42.3",
    "color": "^0.11.3",
    "lodash": "^4.13.1",
    "moment": "^2.13.0",
    "native-base": "2.1.0-rc.2",
    "react-native-button": "^1.6.0",
    "react-native-gifted-messenger": "^0.1.4",
    "react-native-gifted-spinner": "0.0.5",
    "react-native-modalbox": "^1.3.7",
    "react-native-scrollable-tab-view": "^0.7.2",
    "react-native-router-flux": "^3.38.0",
    "react-redux": "^4.4.5",
    "redux": "^3.5.2",
    "redux-persist": "^3.2.2",
    "redux-thunk": "^2.1.0",
    "remote-redux-devtools": "^0.3.3",
    "remote-redux-devtools-on-debugger": "^0.4.6"
  },
  "devDependencies": {
    "react-native-scripts": "0.0.26",
    "jest-expo": "^0.3.0",
    "react-test-renderer": "~15.4.1",
    "chai": "^3.5.0",
    "babel-eslint": "^6.1.2",
    "eslint": "^3.5.0",
    "eslint-config-airbnb": "^11.1.0",
    "eslint-plugin-import": "^1.14.0",
    "eslint-plugin-jsx-a11y": "^2.2.1",
    "eslint-plugin-react": "^6.2.0",
    "eslint-plugin-react-native": "^2.0.0",
    "mocha": "^2.5.3"
  },
  "main": "./node_modules/react-native-scripts/build/bin/crna-entry.js",
  "scripts": {
    "postinstall": "remotedev-debugger",
    "start": "react-native-scripts start",
    "eject": "react-native-scripts eject",
    "android": "react-native-scripts android",
    "ios": "react-native-scripts ios",
    "eslint": "eslint",
    "test": "node node_modules/jest/bin/jest.js --watch"
  },
  "upstreamRepo": "git@gitstrap.com:strapmobile/NativeStarterPro-seed.git",
  "jest": {
    "preset": "jest-expo"
  }
}</code></pre>
