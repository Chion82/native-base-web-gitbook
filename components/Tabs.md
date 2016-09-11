Tabs
----
Tabs are a horizontal region of buttons or links that allow for a consistent navigation experience between screens. It can contain any combination of text and icons, and is a popular method for enabling mobile navigation.
Replacing Component: react-native-scrollable-tab-view `<ScrollableTabView>`

*Syntax*
```JavaScript
import React, { Component } from 'react';
import { Container, Content, Header, Title, Tabs, Text } from 'native-base';

export default class TabsExample extends Component {
  render() {
    return (
      <Container>
        <Content>
          <Tabs>
            <Text tabLabel='One'>Tab1</Text>
            <Text tabLabel='Two'>Tab2</Text>
            <Text tabLabel='Three'>Tab3</Text>
          </Tabs>
        </Content>
      </Container>
    );
  }
}
```

<div class="demo-phone">
  <iframe src="http://localhost:3000/#/app/27"></iframe>
</div>


### Configuration
|Property|Default|Option|Description|
|--------|-------|------|-----------|
|tabLabel|-|-|Name for each tab|
