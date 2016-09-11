Thumbnail
---------
Thumbnail component works very similar to Image. It helps you to showcase an image with various dimensions and shapes. By default, Thumbnail renders an image in circular shape.
Replacing Component: React Native `<Image>`

*Syntax*
```JavaScript
import React, { Component } from 'react';
import { Container, Content, Header, Title, Thumbnail } from 'native-base';

export default class ThumbnailExample extends Component {
  render() {
    return (
      <Container>
        <Content>
          <Thumbnail source={require('../assets/react-native-web.png')} />
          <Thumbnail size={80} source={require('../assets/react-native-web.png')} />
          <Thumbnail square source={require('../assets/react-native-web.png')} />
          <Thumbnail square size={80} source={require('../assets/react-native-web.png')} />
        </Content>
      </Container>
    );
  }
}
```
<div class="demo-phone">
  <iframe src="http://localhost:3000/#/app/28"></iframe>
</div>

### Configuration
|Property|Default|Option|Description|
|--------|-------|------|-----------|
|source|-|-|Image path for thumbnail.|
|square|-|-|Represents shape of thumbnail. By default thumbnail is circle in shape.|
|size|30|user-defined|Dimension of thumbnail.|
