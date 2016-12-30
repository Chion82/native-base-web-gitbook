Icon
----
*Choose from 700+ Icons...*
Perfect, crisp, high definition icons and pixel ideal fonts powered by NativeBase to preserve matters very high first-rate. You will continually have pixel perfect icons on your initiatives.

**IMPORTANT**
* `Icon` for `native-base-web` is re-implemented with [react-icons](https://github.com/gorangajic/react-icons).
* Currently supported icon families: Ionicons(default), FontAwesome, MaterialIcons.
* Not all icons available in NativeBase are supported, check [react-icons source](https://github.com/gorangajic/react-icons) to search for icon names.
* New feature for native-base-web: `Icon.TabBarItem`.

*Syntax*
```JavaScript
import React, { Component } from 'react';
import { Container, Content, Icon } from 'native-base';

export default class IconExample extends Component {
  render() {
    return (
      <Container>
        <Content>
          <Icon name='ios-home' />
          <Icon name='ios-person' style={{fontSize: 20, color: 'red'}}/>
        </Content>
      </Container>
    );
  }
}
```
* Icon takes two attributes: `name`, `style`.
* In case if you want to include icon with custom color, size etc then that should go into `style`.
* All the icons in the icon libraries of NativeBase, are scalable vector icons that can be customized size, color, etc.

### Configuration
|Property|Default|Option|Description|
|--------|-------|------|-----------|
|name|-|-|Name of the icon.|
|color|black|user-defined|Renders icon with defined color. Note: Include this prop within style|
|fontSize|27|user-defined|Renders icon with defined icon-size. Note: Include this prop within style|

## Icon.TabBarItem
Use with `TabBarIOS`. This feature is migrated from [react-native-vector-icons](https://github.com/oblador/react-native-vector-icons).
Only available when using [react-native-web-extended](https://github.com/Chion82/react-native-web-extended).

*Syntax*
```JavaScript
import { View, Text, TabBarIOS } from 'react-native';
import { Icon } from 'native-base';

function TabBarView(props) {
  return (
    <TabBarIOS>
      <Icon.TabBarItem
        title="Home"
        iconName="ios-home-outline"
        selectedIconName="ios-home"
        >
        <View style={styles.tabContent}><Text>Home Tab</Text></View>
      </Icon.TabBarItem>
    </TabBarIOS>
  );
}
```
