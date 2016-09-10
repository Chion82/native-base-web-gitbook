Card
----
Card is a pure NativeBase component.
Card is a flexible and extensible content container. It includes options for headers and footers, a wide variety of content, contextual background colors, and powerful display options.
NativeBase Cards support a wide variety of content, including images, text, list groups, links, and more. Mix and match multiple content types to create the card you need.

Contents:
* Card Header and Footer
* Card List
* Card Image
* Card Showcase
* Card OnClick

*General Syntax*
```JavaScript

import React, { Component } from 'react';
import { Container, Content, Card, CardItem, Text } from 'native-base';

export default class CardExample extends Component {
  render() {
    return (
      <Container>
        <Content>
          <Card>
            <CardItem>                        
              <Text>
                  //Your text here
              </Text>
            </CardItem>
          </Card>
        </Content>
      </Container>
    );
  }
}
```

<div class="demo-phone">
	<iframe src="http://localhost:3000/#/app/8"></iframe>
</div>

* `Card`: This component adds a box-shadow by default. Also provides default spacing and alignment between cards.
* `CardItem`: This is the child component of Card. Works very similar to the list items of list. Card takes any number of CardItem.
* CardItem component takes input such as: Text, Button, Image, Thumbnail, Icon.
* Replacing Component for Card: React Native `<View>`
* Replacing Component for CardItem: React Native `<View>`

### Configuration
|Property|Default|Option|Description|
|--------|-------|------|-----------|
|header|-|-|Displays both as header and footer for cards.|
|note|-|-|Sub caption for Card header.|
|cardBody|-|-|Defines section for body of card.The child components are rendered with proper spacing and alignment.|
|button|-|-|To navigate on click of a card item.|


## Card Header and Footer
To add an optional header and/or footer within a card, include `header` prop with the `CardItem`.
* **Card Header**: Include `header` prop with first instance of CardItem within Card.
* **Card Footer**: Include `header` prop with last instance of CardItem within Card.

*Syntax*
```JavaScript
import React, { Component } from 'react';
import { Container, Content, Card, CardItem, Text } from 'native-base';

export default class CardHeaderFooterExample extends Component {
  render() {
    return (
      <Container>
        <Content>
          <Card>
            <CardItem header>                        
            <Text>Card Header</Text>
            </CardItem>

            <CardItem>                        
            <Text>
            //Your text here
            </Text>
            </CardItem>

            <CardItem header>                        
            <Text>Card Footer</Text>
            </CardItem>
          </Card>
        </Content>
      </Container>
    );
  }
}
```

<div class="demo-phone">
	<iframe src="http://localhost:3000/#/app/9"></iframe>
</div>

## Card List
Include `CardItem` subsequently within `Card` to create a card with lists.

*Syntax*
```JavaScript
import React, { Component } from 'react';
import { Container, Content, Card, CardItem, Text, Icon } from 'native-base';

export default class CardListExample extends Component {
  render() {
    return (
      <Container>
        <Content>
          <Card>
            <CardItem>
              <Icon name='social-google' />
              <Text>Google</Text>
            </CardItem>
            <CardItem>
              <Icon name='social-facebook' />
              <Text>Facebook</Text>
            </CardItem>
            <CardItem>
              <Icon name='social-instagram' />
              <Text>Instagram</Text>
            </CardItem>
          </Card>
        </Content>
      </Container>
    );
  }
}
```

<div class="demo-phone">
	<iframe src="http://localhost:3000/#/app/10"></iframe>
</div>

## Card Image
Want to have something more with Card Lists?
Include image with `CardItem` within `Card` along with some text before and after image to create a card with lists.
Here is your Card Image ready !

*Syntax*
```JavaScript
import React, { Component, Image } from 'react';
import { Container, Content, Card, CardItem, Thumbnail, Text, Icon } from 'native-base';
​
export default class CardImageExample extends Component {
  render() {
    return (
      <Container>
        <Content>
          <Card>
            <CardItem>
              <Thumbnail source={require('./img/guitar.jpeg')} />
              <Text>Instrumental Songs</Text>
              <Text note>Guitar</Text>
            </CardItem>

            <CardItem>                        
              <Image style={{ resizeMode: 'cover' }} source={require('./img/music.png')} />
            </CardItem>

            <CardItem>
              <Icon name='ios-musical-notes' style={{color : '#ED4A6A'}} />
              <Text>Listen now</Text>                        
            </CardItem>
         </Card>
        </Content>
      </Container>
    );
  }
}
```

<div class="demo-phone">
	<iframe src="http://localhost:3000/#/app/11"></iframe>
</div>

## Card Showcase
Card Showcase is further customization of Card Image. It uses several different items.

* Begins with the Card List component, which is similar to out List Avatar.
* `cardBody` prop for images and text.

*Syntax*
```JavaScript
import React, { Component, Image } from 'react';
import { Container, Content, Card, CardItem, Thumbnail, Text, Button } from 'native-base';

export default class CardShowcaseExample extends Component {
  render() {
    return (
      <Container>
        <Content>
          <Card>
            <CardItem >                       
              <Thumbnail source={require('./img/nativeBase-logo.png')} />
              <Text>NativeBase</Text>
              <Text note>April 15, 2016</Text>
            </CardItem>

            <CardItem cardBody>
              <Image style={{ resizeMode: 'cover' }} source={require('./img/wallpaper.png')} />
              <Text>
              //Your text here
              </Text>
              <Button transparent textStyle={{color: '#87838B'}}>
                389 Stars
              </Button>
            </CardItem>
          </Card>
        </Content>
      </Container>
    );
  }
}
```

<div class="demo-phone">
	<iframe src="http://localhost:3000/#/app/12"></iframe>
</div>
