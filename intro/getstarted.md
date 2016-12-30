Quick Start
-----------
It's advised to use [our boilerplate](https://github.com/Chion82/rnweb-native-base-starter) to initialize your app structure.

### Setup
```
git clone https://github.com/Chion82/rnweb-native-base-starter.git my-react-app
cd my-react-app
npm i
```

### Develop
The API service for this todo-starter app is powered by a simple backend server. Run it by
```
npm run backend
```
Then open a new terminal and run your app:
```
npm run dev
```

### Build & Deploy
Build your app in production mode to significantly improve render performance.
```
npm run build
```
Then deploy files under the `dist` directory on your server.

Manual Setup
------------
Install `native-base-web`:

```
npm install --save native-base-web
```

native-base-web is depended on [react-native-web](https://github.com/necolas/react-native-web). Install it if you have not yet configured your app structure:

```
npm install --save react-native-web
```

Setup resolve alias in your webpack configuration:

```JavaScript
resolve: {
	alias: {
		'react-native': 'react-native-web',
		'native-base' : 'native-base-web',
		'react/lib/ReactNativePropRegistry': 'react-native-web/dist/modules/ReactNativePropRegistry'
	}
}
```

Alternatively, you can use [react-native-web-extended](https://github.com/Chion82/react-native-web-extended) instead of [react-native-web](https://github.com/necolas/react-native-web) for extended components and APIs, in which case your webpack configuration should be:

```JavaScript
resolve: {
	alias: {
		'react-native': 'react-native-web-extended',
		'native-base': 'native-base-web',
		//Icon.TabBarItem
		'react-native-vector-icons/Ionicons': 'native-base-web/lib/Components/Widgets/Icon',
		'react/lib/ReactNativePropRegistry': 'react-native-web-extended/dist/modules/ReactNativePropRegistry'
	}
}
```
