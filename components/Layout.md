Layout
------
The layout system is an essential concept that needs to be mastered in order to create great layouts and UIs. React Native uses Flexbox to create the layouts, which is great when we need to accommodate our components and views in different screen sizes or even different devices. Flexbox is awesome but it could be tiresome for newbies.

*Not being very good at Flexbox?
Here comes the [Easy Grid](https://github.com/GeekyAnts/react-native-easy-grid) of NativeBase, a wrapper of Flexbox. *

The layout system in NativeBase is very powerful and flexible. No more worries about props of Flexbox such as alignItems, flexDirection, justifyContent, margin, padding, position, width etc. You can create any layout with all the available options that we have. In order to build custom layouts and components, understanding how layout works in NativeBase is not as hard as Flexbox. Flexbox makes it look like percentages, however what actually is happening is just ratios. On the easier part, ratios are easier to represent than percentage/decimals. For this reason, the Easy Grid takes in ratios in place of percentage.
Performance wise, Easy Grid is noteworthy and works as fine as Flexbox, not much of calculation.

*Syntax*
```JavaScript
import React, { Component } from 'react';
import { Container, Content } from 'native-base';
import { Col, Row, Grid } from 'react-native-easy-grid';

export default class LayoutExample extends Component {
  render() {
    return (
      <Container>
        <Content>
          <Grid>
            <Col style={{ backgroundColor: '#D954D7', height: 200 }}></Col>
            <Col style={{ backgroundColor: '#D93735', height: 200  }}></Col>
          </Grid>
        </Content>
      </Container>
    );
  }
}
```

<div class="demo-phone">
	<iframe src="https://blog.chionlab.moe/native-base-web-example/#/app/16"></iframe>
</div>

NOTE: `<Content>` component uses `<ScrollView>`. This is required by `<Col>` and `<Row>` elements of Easy-Grid to have a defined height.

* Replacing Component for Grid: React Native `<View>`
* Replacing Component for Col: React Native `<View>`
* Replacing Component for Row: React Native `<View>`
