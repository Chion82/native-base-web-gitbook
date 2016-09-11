List
----
This component is completely built by NativeBase.
A base component for specifying lists of information. List must contain one or more list elements. Props provide configurability for several features. Provides a number of attributes that follows styling and interaction guidelines for each platform, so that they are intuitive for users to interact with.

**Contents:**
* List Divider
* List Icon
* List Avatar
* List Thumbnail
* Dynamic List
* List OnClick

*Syntax*
```JavaScript
import React, { Component } from 'react-native';
import { Container, Content, List, ListItem, Text } from 'native-base';
​
export default class ListExample extends Component {
  render() {
    return (
      <Container>
        <Header>
          <Title>List</Title>
        </Header>
        <Content>
          <List>
            <ListItem >
              <Text>Simon Mignolet</Text>
            </ListItem>
            <ListItem>
              <Text>Nathaniel Clyne</Text>
            </ListItem>
            <ListItem>
              <Text>Dejan Lovren</Text>
            </ListItem>
          </List>
        </Content>
      </Container>
    );
  }
}
```

<div class="demo-phone">
	<iframe src="http://localhost:3000/#/app/17"></iframe>
</div>

* `List`: This component defines a section to include your list items.
* `ListItem`:
  - This is the child component of List.
  - Defines a list item.
  - Adds border at bottom of each ListItem.
  - List takes any number of ListItem.
* ListItem component takes input such as: Text, Badge, Thumbnail, Icon.
* Replacing Component for List: React Native `<View>`
* Replacing Component for ListItem: React Native `<View>`

### Configuration
|Property|Default|Option|Description|
|--------|-------|------|-----------|
|itemDivider|-|-|Helps to organize and group the list items.|
|note|-|-|Sub caption for List Item.|
|iconLeft|true|true false|Aligns icon to the left of ListeItem.|
|iconRight|true|true false|Aligns icon to the right of ListeItem.|
|dataArray|Array|user-defined array|Array of data chunks to render iteratively.|
|renderRow|Function|-|Callback which takes a chunk of data from dataArray and returns as a component.|
|button|-|-|To navigate on click of a list item.|

## List Divider
The List Divider component creates a list separator, which can be used for grouping list items. To create a divider for any child element of the list, include `itemDivider` prop with `ListItem` component. The List Divider of NativeBase comes with default style which is easily customisable.

*Syntax*
```JavaScript
import React, { Component } from 'react';
import { Container, Content, List, ListItem, Text } from 'native-base';

export default class ListDividerExample extends Component {
  render() {
    return (
      <Container>
        <Content>
          <List>
            <ListItem itemDivider>
              <Text>Goalkeeper</Text>
            </ListItem>                    
            <ListItem >
              <Text>Simon Mignolet</Text>
            </ListItem>
            <ListItem itemDivider>
              <Text>Defenders</Text>
            </ListItem>  
            <ListItem>
              <Text>Nathaniel Clyne</Text>
            </ListItem>
            <ListItem>
              <Text>Dejan Lovren</Text>
            </ListItem>
          </List>
        </Content>
      </Container>
    );
  }
}
```
<div class="demo-phone">
	<iframe src="http://localhost:3000/#/app/18"></iframe>
</div>

## List Icon
Lists can have icons assigned either to the left and/or right side of each list item. Along with icons, list item can also have badges assigned. To have note kind of text for list item, include `note` prop with `Text` component of `ListItem`.

*Syntax*
```JavaScript
import React, { Component } from 'react-native';
import { Container, Content, List, ListItem, Text, Icon, Badge } from 'native-base';

export default class ListIconExample extends Component {
  render() {
    return (
      <Container>
        <Content>
          <List>
            <ListItem iconLeft>
              <Icon name='ios-chatboxes' />
              <Text>Simon Mignolet</Text>
            </ListItem>
            <ListItem iconLeft>
              <Icon name='ios-alarm' />
              <Text>Nathaniel Clyne</Text>
              <Badge>2</Badge>
            </ListItem>
            <ListItem iconLeft>
              <Icon name='md-notifications' />
              <Text>Dejan Lovren</Text>
              <Text note>Note here</Text>
            </ListItem>
            <ListItem iconLeft iconRight>
              <Icon name='ios-mic' />
              <Text>Mama Sakho</Text>
              <Icon name='ios-mic-outline' />
            </ListItem>
          </List>
        </Content>
      </Container>
    );
  }
}
```
<div class="demo-phone">
	<iframe src="http://localhost:3000/#/app/19"></iframe>
</div>

## List Avatar
List Avatars are medium to showcase an image with your list item whose dimension lays between icon and dimension. To create a avatar list, nest `<Thumbnail>` component within `<ListItem>` component.

*Syntax*
```JavaScript
import React, { Component } from 'react-native';
import { Container, Content, List, ListItem, Thumbnail, Text } from 'native-base';

export default class ListAvatarExample extends Component {
  render() {
    return (
      <Container>
        <Content>
          <List>
            <ListItem>
              <Thumbnail source={require('./img/hyundai-logo.png')} />
              <Text>Hyundai</Text>
              <Text note>1967</Text>
            </ListItem>
            <ListItem>
              <Thumbnail source={require('./img/fiat-logo.jpg')} />
              <Text>Fiat</Text>
              <Text note>2007</Text>
            </ListItem>
          </List>
        </Content>
      </Container>
    );
  }
}
```
<div class="demo-phone">
	<iframe src="http://localhost:3000/#/app/20"></iframe>
</div>

## List Thumbnail
List Thumbnails are medium to exhibit an image with your list item. To create a thumbnail list, nest `<Thumbnail>` component within `<ListItem>` component with few props and style.

*Syntax*
```JavaScript
import React, { Component } from 'react-native';
import { Container, Content, List, ListItem, Thumbnail, Text } from 'native-base';

export default class ListThumbnailExample extends Component {
  render() {
    return (
      <Container>
        <Content>
          <List>
            <ListItem>
              <Thumbnail square size={80} source={require('./img/hyundai-logo.png')} />
              <Text>Hyundai</Text>
              <Text note>1967</Text>
            </ListItem>
            <ListItem>
              <Thumbnail square size={80} source={require('./img/infiniti-logo.jpg')} />
              <Text>Infiniti</Text>
              <Text note>1989</Text>
            </ListItem>
          </List>
        </Content>
      </Container>
    );
  }
}
```
<div class="demo-phone">
	<iframe src="http://localhost:3000/#/app/21"></iframe>
</div>
