Form
----
NativeBase makes use of `List` to design Forms that include group of related input components. Include any combination of NativeBase components to make up your form.

*Syntax*
```JavaScript
import React, { Component } from 'react';
import { Container, Content, List, ListItem, InputGroup, Input, Icon } from 'native-base';

export default class FormExample extends Component {
  render() {
    return (
      <Container>
        <Content>
          <List>
            <ListItem>
              <InputGroup>
                <Icon name='ios-person' />
                <Input placeholder='EMAIL' />
              </InputGroup>
            </ListItem>

            <ListItem>
              <InputGroup>
                <Icon name='ios-unlocked' />
                <Input placeholder='PASSWORD' secureTextEntry={true}/>
              </InputGroup>
            </ListItem>

            <ListItem>
              <InputGroup >
                <Input inlineLabel label='NAME' placeholder='John Doe' />
              </InputGroup>
            </ListItem>

            <ListItem>
              <InputGroup >
                <Input stackedLabel label='Address Line 1' placeholder='Address' />
              </InputGroup>
            </ListItem>
          </List>
        </Content>
      </Container>
    );
  }
}
```

<div class="demo-phone">
	<iframe src="https://blog.chionlab.moe/native-base-web-example/#/app/14"></iframe>
</div>

### Configuration
|Property|Default|Option|Description|
|--------|-------|------|-----------|
|inlineLabel|-|-|Label placed to the left of the input element. When the user enters text, the label does not hide. This can also be used along with placeholder.|
|stackedLabel|-|-|Places the label on top of the input element which appears like a stack. This can also be used along with placeholder.|
