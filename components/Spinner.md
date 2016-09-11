Spinner
-------
If you have certain screens of your app that take some time to load, you may want to consider a page loader. A page loader is any kind of animation that visually communicates to a visitor that the page is loading and to just sit tight for a few seconds. Without a page loader, user might think that the app is being unresponsive and just click away in frustration. A page loader also provides a small distraction which can actually makes the wait seem much shorter.
Replacing Component: React Native `<ActivityIndicator>`

*Syntax*
```JavaScript
import React, { Component } from 'react';
import { Container, Content, Header, Title, Spinner } from 'native-base';

export default class SpinnerExample extends Component {
  render() {
    return (
      <Container>
        <Content>
          <Spinner />
          <Spinner color='red' />
          <Spinner color='green' />
          <Spinner color='blue' />
        </Content>
      </Container>
    );
  }
}
```

<div class="demo-phone">
  <iframe src="https://blog.chionlab.moe/native-base-web-example/#/app/26"></iframe>
</div>

### Configuration
|Property|Default|Option|Description|
|--------|-------|------|-----------|
|color|#45D56E|user-defined|Color of Spinner.|
