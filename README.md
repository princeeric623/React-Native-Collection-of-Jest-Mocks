# React Native Jest Mocks

Collection of Jest mocks for React Native that I use for different projects.

## Usage

1.- First, install the package.

`yarn add --dev react-native-jest-mocks`

or

`npm install --save-dev react-native-jest-mocks`

2.- If you haven't already, create a `jest-setup.js` file in the root of your project.

3.- Afterwards, inside your package.json file, in the `jest` section, reference your setup file:

````
"jest": {
  "preset": "react-native",
  "setupFiles": [
    "./jest-setup.js"
  ]
}
````

4.- Now, inside your `jest-setup.js` file import the module:

`import mocks from 'react-native-jest-mocks'`

5.- And init the mocks:

`mocks.initAll();`

Mocks currently included:

* navigator global
* Linking
* ScrollView
* YellowBox
* `react-native-localize`
* console.error: This is currently included to avoid some warnings from react-navigation.

## License
MIT
