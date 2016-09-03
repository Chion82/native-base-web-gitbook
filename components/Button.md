Button
------
Button is a pure NativeBase component.
Buttons are the integral part of an application. They are used for various purposes like, submit or reset a form, navigate, performing interactive actions such as showing or hiding something in an app on click of the button, etc.

Contents:
* Button Theme
* Block Button
* Rounded Button
* Icon Button
* Outline Button
* Transparent Button
* Button Size
* Disabled Button

*Syntax*
```JavaScript
import React, { Component } from 'react';
import { Container, Content, Button, Header, Title } from 'native-base';

export default class ButtonExample1 extends Component {
  render() {
    return (
      <Container>
				<Header>
					<Title>Button</Title>
				</Header>
        <Content>
          <Button> Click Me! </Button>
        </Content>
      </Container>
    );
  }
}

```

<div class="demo-phone">
		<iframe src="http://localhost:3000/#/app/4"></iframe>
</div>

* NativeBase provides `Button` component which is readily not available in React Native.
* Supports React Native app on both iOS and Android devices.
* Button component takes input such as: Text, Icon, Text with Icon.
* NativeBase gives you privilege to customize the props of this component.
 	*Example*: To have custom style for button, include them in `style` prop of button.
* Intakes user-defined styles.
* NativeBase has provided its users with enormous list of `props` that can be used with Button.
* *Replacing Component*: React Native `<TouchableOpacity>`

### Configuration
|Property|Default|Option|Description|
|--------|-------|------|-----------|
|style|-|-|Defines button style|
|textStyle|-|-|Defines button text style|
|block|-|-|Block level button|
|rounded|-|-|Renders button with slightly round shaped edges.|
|bordered|-|-|Applies outline button style.|
|transparent|-|-|Gives you effect of Icon-buttons.To have button with transparent background, include this prop.|
|small|-|-|For small size button|
|large|-|-|For large size button|
|iconLeft|-|-|Used for Icon alignment.Aligns icon to the left in button.By default, icons are aligned to the left in button.|
|iconRight|-|-|Used for Icon alignment.Aligns icon to the right in button.|
|disabled|false|true false|Disables click option for button|

### Button Theme
NativeBase provides buttons with wide range of colors, size and variuos other props.
NativeBase provides following color themes:

* Primary (default)
* Success
* Info
* Warning
* Danger

*Syntax*
```JavaScript
import React, { Component } from 'react';
import { Container, Content, Button, Header, Title } from 'native-base';

export default class ButtonExample2 extends Component {
  render() {
    return (
      <Container>
				<Header>
					<Title>Button</Title>
				</Header>
        <Content>
          <Button primary> Primary </Button>
          <Button success> Success </Button>
          <Button info> Info </Button>
          <Button warning> Warning </Button>
          <Button danger> Danger </Button>
        </Content>
      </Container>
    );
  }
}
```
<div class="demo-phone">
		<iframe src="http://localhost:3000/#/app/5"></iframe>
</div>

### Block Button
A block level button spans the entire width of the parent element. Create block level buttons by adding `block` prop with the `Button`.

*Syntax*
```JavaScript
import React, { Component } from 'react';
import { Container, Content, Button, Header, Title } from 'native-base';

export default class ButtonExample3 extends Component {
  render() {
    return (
      <Container>
				<Header>
					<Title>Button</Title>
				</Header>
        <Content>
          <Button block> Primary </Button>
          <Button block success> Success </Button>
          <Button block info> Info </Button>
          <Button block warning> Warning </Button>
          <Button block danger> Danger </Button>
        </Content>
      </Container>
    );
  }
}
```
<div class="demo-phone">
		<iframe src="http://localhost:3000/#/app/6"></iframe>
</div>
