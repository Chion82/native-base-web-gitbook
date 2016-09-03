NativeBase for Web
------------------
[![npm version](https://badge.fury.io/js/native-base-web.svg)](https://badge.fury.io/js/native-base-web)

NativeBase-web is a project to bring [NativeBase](http://nativebase.io/) components to the Web, with the help of [react-native-web-extended](https://github.com/Chion82/react-native-web-extended).

Get Started
-----------
To install:

```
npm install --save native-base-web
```

NativeBase-web is depended on react-native-web-extended, an extended version of [react-native-web](https://github.com/necolas/react-native-web). Install it if you have not yet configured your app structure:

```
npm install --save react-native-web-extended
```

Setup resolve alias in your webpack configuration:

```JavaScript
resolve: {
	alias: {
		'react-native': 'react-native-web-extended',
		'native-base' : 'native-base-web'
	}
}
```
