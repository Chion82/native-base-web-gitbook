Search Bar
----------
It’s kind of common on the Internet where – if we fail to get what we are looking for on a website, we resort to searching. Search box has always been an essential part of any application. We provide you with the one, which filters the list based on your search input.

*Syntax*
```JavaScript
import React, { Component } from 'react';
import { Container, Content, Header, Button, InputGroup, Input, Icon } from 'native-base';

export default class SearchBarExample extends Component {
  render() {
    return (
      <Container>
        <Header searchBar rounded>
          <InputGroup>
            <Icon name='ios-search' />
            <Input placeholder='Search' />
            <Icon name='ios-people' />
          </InputGroup>
          <Button transparent>
            Search
          </Button>
        </Header>
      </Container>
    );
  }
}
```

<div class="demo-phone">
  <iframe src="http://localhost:3000/#/app/25"></iframe>
</div>

* `searchBar`: Prop to be used with `<Header>` component to have Search bar onto the Header section of your screen.
* Replacing Component: React Native `<View>`

### Configuration
|Property|Default|Option|Description|
|--------|-------|------|-----------|
|rounded|regular|-|Wraps the search bar with predefined border options.|
