Theming NativeBase-web Apps
---------------------------
Customizing NativeBase-web themes is just the same way as NativeBase. But there is something you need to notice:
* Use [themes/light.js from NativeBase](https://github.com/GeekyAnts/NativeBase/blob/master/Components/Themes/light.js) to start theming. Don't use that one from `native-base-web`, as we changed the theme object to a function which will not work in NativeBase when migrating code to workaround an issue.
* In NativeBase-web projects, the value of `Platform.OS` from `react-native-web(-extended)` is always `web`. So take care when modifying your copied `light.js`, as there are many conditions checking `Platform.OS` by default.
* NativeBase provides both IOS and Android(material) themes, so does NativeBase-web. In your `PROJECT_ROOT/index.web.js`, add the code bolow to choose one of them:

```JavaScript
import { OSTheme } from 'native-base';

OSTheme.setOSTheme('android'); //Default: 'ios'
```

For detailed customizing guide, check out [NativeBase official documentation](http://nativebase.io/docs/v0.5.7/customize#themingNativeBaseApp).
