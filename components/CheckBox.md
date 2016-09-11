Check Box
---------
Check Box allows the user to select a number of items from a set of choices.
Replacing Component: React Native `<View>`

*Syntax*
```JavaScript
import React, { Component } from 'react';
import { Container, Content, List, ListItem, Text, CheckBox } from 'native-base';

export default class CheckBoxExample extends Component {
  render() {
    return (
      <Container>
        <Content>
          <List>
            <ListItem>
              <CheckBox checked={true} />
              <Text>Daily Stand Up</Text>
            </ListItem>
            <ListItem>
              <CheckBox checked={false} />
              <Text>Discussion with Client</Text>
            </ListItem>
          </List>
        </Content>
      </Container>
    );
  }
}
```

<div class="demo-phone">
	<iframe src="https://blog.chionlab.moe/native-base-web-example/#/app/13"></iframe>
</div>

### Configuration
|Property|Default|Option|Description|
|--------|-------|------|-----------|
|checked|false|true, false|Represents the state value of an item from set of choices.|
