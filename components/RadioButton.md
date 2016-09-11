Radio Button
------------
Radio buttons let the user select any one from a set of options.
Replacing Component: React Native `<View>`

*Syntax*
```JavaScript
import React, { Component } from 'react';
import { Container, Content, List, ListItem, Text, Radio } from 'native-base';

export default class RadioButtonExample extends Component {
  render() {
    return (
      <Container>
        <Content>
          <List>
            <ListItem>
              <Radio selected={false} />
              <Text>Daily Stand Up</Text>
            </ListItem>
            <ListItem>
              <Radio selected={true} />
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
	<iframe src="https://blog.chionlab.moe/native-base-web-example/#/app/24"></iframe>
</div>

### Configuration
|Property|Default|Option|Description|
|--------|-------|------|-----------|
|selected|false|true false|Represents the state value of an item from set of choices.|
