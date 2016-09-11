Badge
-----
All of us must have seen notification badges somewhere, such as on smart phones or facebook. NativeBase is here to include this into your collection of readymade components. Badges are numerical indicators of how many items are associated with an element. Badges can notify you that there are new or unread messages or notifications. These can be very effective in alerting the user to new things on your app.

*Syntax*
```JavaScript
import React, { Component } from 'react';
import { Container, Content, Badge, Header, Title } from 'native-base';

export default class BadgeExample extends Component {
	render() {
		return (
			<Container>
				<Header>
					<Title>Badge Example</Title>
				</Header>
				<Content>
					<Badge>2</Badge>
					<Badge primary>2</Badge>
					<Badge success>2</Badge>
					<Badge info>2</Badge>
					<Badge warning>2</Badge>
					<Badge danger>2</Badge>
				</Content>
			</Container>
		);
	}
}
```

<div class="demo-phone">
		<iframe src="https://blog.chionlab.moe/native-base-web-example/#/app/3"></iframe>
</div>
