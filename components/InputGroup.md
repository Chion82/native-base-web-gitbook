Input Group
-----------
This is a NativeBase component built on top of React Native's `<TextInput>`.
A foundational component for inputting text into the app via a keyboard. Props provide configurability for several features, such as auto-correction, auto-capitalization, placeholder text, and different keyboard types, such as a numeric keypad. Provides a number of attributes that follows styling and interaction guidelines for each platform, so that they are intuitive for users to interact with.

**Contents:**
Regular Textbox
Underlined Textbox
Rounded Textbox
Icon Textbox
Success Input Textbox
Error Input Textbox
Disabled Textbox

*General Syntax*
```JavaScript
import React, { Component } from 'react';
import { Container, Content, InputGroup, Input } from 'native-base';

export default class InputGroupExample extends Component {
  render() {
    return (
      <Container>
        <Content>
          <InputGroup>
            <Input />
          </InputGroup>
        </Content>
      </Container>
    );
  }
}
```

* NativeBase extends React Native's `<TextInput/>` by adding several attributes and props to `<Input />`.
* NativeBase defines textbox for you, by just defining `<Input />` in your app.
* Supports custom styles on both iOS and Android devices.
* InputGroup component renders elements such as: Text, Input, Icon.
* The props of `<TextInput>` are smoothly applicable to` <Input>`.
* InputGroup also takes in props value.
* Replacing Component for InputGroup: React Native `<View>`
* Replacing Component for Input: React Native `<TextInput>`

<div class="demo-phone">
	<iframe src="http://localhost:3000/#/app/15"></iframe>
</div>

### Configuration
|Property|Default|Option|Description|
|--------|-------|------|-----------|
|placeholder|-|-|The string that will be rendered before text input has been entered. Optional user-defined placeholder for textbox.|
|borderType|underline|regular, underline,rounded|Wraps the textbox with predefined border options.|
|secureTextEntry|false|true, false|If true, the text input obscures the text entered so that sensitive text like passwords stay secure.This prop can be passed to `<Input>`.|
|iconRight|true|true,false|If true, the icon in the input text box appears to the right.|
|success|-|-|The border color of textbox for valid input.|
|error|-|-|The border color of textbox for invalid input.|
|disabled|-|-|Disables inputting data.|

## Regular Textbox
To use the regular textbox which is rectangular in shape, include the `borderType` property and assign it with value as **regular**.

*Syntax*
```JavaScript
import React, { Component } from 'react';
import { Container, Content, InputGroup, Input } from 'native-base';

export default class RegularTextboxExample extends Component {
  render() {
    return (
      <Container>
        <Content>​
          // Simple rectangular text input box
          <InputGroup borderType='regular' >
            <Input placeholder='Type your text here'/>
          </InputGroup>
        </Content>
      </Container>
    );
  }
}
```

## Underlined Textbox
To use the underlined textbox, include the `borderType` property and assign it with value as **underline**.

**Syntax**
```JavaScript
import React, { Component } from 'react';
import { Container, Content, InputGroup, Input, Icon } from 'native-base';

export default class UnderlinedTextboxExample extends Component {
  render() {
    return (
      <Container>
        <Content>​
          // Underlined text input box with placeholder text and an icon
          <InputGroup borderType='underline' >
            <Icon name='ios-home' style={{color:'#384850'}}/>
            <Input placeholder='Type your text here' />
          </InputGroup>
        </Content>
      </Container>
    );
  }
}
```

## Rounded Textbox
To have a textbox with round type border, include the `borderType` property and assign it with value as **rounded**.

*Syntax*
```JavaScript
import React, { Component } from 'react';
import { Container, Content, InputGroup, Input, Icon } from 'native-base';

export default class RoundedTextboxExample extends Component {
  render() {
    return (
      <Container>
        <Content>
          // Rounded text input box with icon
          <InputGroup borderType='rounded' >
            <Icon name='ios-home' style={{color:'#384850'}}/>
            <Input placeholder='Type your text here'/>
          </InputGroup>
        </Content>
      </Container>
    );
  }
}
```

## Icon Textbox
Icons can be easily added to the NativeBase Textbox. To do so, include an icon within the `<InputGroup>`.
By default the icon will be aligned to the left in the textbox.
However, you can also render icon to the right. To display icon at the end of textbox, include `iconRight` prop with the `<InputGroup>`.

*Syntax*
```JavaScript
import React, { Component } from 'react';
import { Container, Content, InputGroup, Input, Icon } from 'native-base';
​
export default class IconTextboxExample extends Component {
  render() {
    return (
      <Container>
        <Content>
          // Text input box with icon aligned by default to the left
          <InputGroup>
            <Icon name='ios-home' style={{color:'#00C497'}}/>
            <Input placeholder='Icon Textbox'/>
          </InputGroup>

          // Text input box with icon aligned to the right
          <InputGroup iconRight>
            <Icon name='arrow-swap' style={{color:'#00C497'}}/>
            <Input placeholder='Icon Alignment in Textbox'/>
          </InputGroup>
        </Content>
      </Container>
    );
  }
}
```

## Success Input Textbox
To display textbox with valid data, include the `success` prop with `<InputGroup>`.

*Syntax*
```JavaScript
import React, { Component } from 'react';
import { Container, Content, InputGroup, Input, Icon } from 'native-base';

export default class SuccessInputTextboxExample extends Component {
  render() {
    return (
      <Container>
        <Content>
          <InputGroup iconRight success>
            <Icon name='ios-checkmark' style={{color:'#00C497'}}/>
            <Input placeholder='Textbox with Success Input'/>
          </InputGroup>
        </Content>
      </Container>
    );
  }
}
```

## Error Input Textbox
To display textbox with invalid data, include the `error` prop with `<InputGroup>`.

*Syntax*
```JavaScript
import React, { Component } from 'react';
import { Container, Content, InputGroup, Input, Icon } from 'native-base';

export default class ErrorInputTextboxExample extends Component {
  render() {
    return (
      <Container>
        <Content>
          <InputGroup iconRight error>
            <Icon name='ios-close' style={{color:'red'}}/>
            <Input placeholder='Textbox with Error Input'/>
          </InputGroup>
        </Content>
      </Container>
    );
  }
}
```

## Disabled Textbox
To restrict inputting data into textbox, include the `disabled` prop with `<InputGroup>`.

*Syntax*
```JavaScript
import React, { Component } from 'react';
import { Container, Content, InputGroup, Input, Icon } from 'native-base';

export default class DisabledTextboxExample extends Component {
  render() {
    return (
      <Container>
        <Content>
            <InputGroup iconRight disabled>
              <Icon name='ios-information' style={{color: '#384850'}}/>
              <Input placeholder='Disabled Textbox'/>
            </InputGroup>
        </Content>
      </Container>
    );
  }
}
```
