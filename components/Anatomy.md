Anatomy
-------
Automatically animates views to their new positions.
A common way to use NativeBase screen structure is to have all the components within `<Container>`.

Contents:  
`Header`  
`Content`

## Basic Usage

*General Syntax*
```JavaScript
import React, { Component } from 'react';
import { Container, Header, Title, Content } from 'native-base';
import { Text } from 'react-native';

export default class AnatomyExample1 extends Component {
	render() {
		return (
			<Container>
				<Header>
					<Title>Header</Title>
				</Header>

				<Content>
					<Text>This is body section</Text>
				</Content>
			</Container>
		);
	}
}
```

<div style="width:290px;height:593px;margin-left:auto;margin-right:auto;background-image:url(/images/iphone.png)">
		<iframe style="border-width:0px;background-color:white;
		width:337px;height:600px;margin-left:-23px;margin-top:-10px;
		-ms-transform: scale(0.75);
    -moz-transform: scale(0.75);
    -o-transform: scale(0.75);
    -webkit-transform: scale(0.75);
    transform: scale(0.75);
		" src="http://localhost:3000/#/app/1"></iframe>
</div>

* NativeBase provides its own frame component, named after `<Container>`.
* All the components should be included within the Container.
* Container takes mainly two components: `<Header>` and `<Content>`.
* Container comes with its predefined stylesheet, with an added advantage of accepting user-defined styles.
* Usage of Container's Header component is very similar to your HTML `<head>`.
* The Content component of Container is nothing but the body section of your screen.

## Header

* NativeBase component that renders as Header (navbar) for your screen.
* There can be a single Header component into your Container.
* To have Header for your screen, include `<Header>` component within `<Container>`.
* NativeBase gives you flexibility to define your Header component anywhere in the bounds of Container.
* Header takes input as: Button and Title (Text)
* The components those are defined within `<Header>` will be rendered in the same order that you define them.
* Header provides you with stylesheet.
* User can add custom styles while defining `<Header>` within their app.
* Replacing Component: React Native `<View>`

*Syntax*
```JavaScript
import React, { Component } from 'react';
import { Container, Header, Title, Content, Button, Icon } from 'native-base';
import { Text } from 'react-native';

export default class AnatomyExample2 extends Component {
	render() {
		return (
			<Container>
				<Header>
					<Button transparent>
						<Icon name='ios-arrow-back' />
					</Button>

					<Title>Header</Title>

					<Button transparent>
						<Icon name='md-menu' />
					</Button>
				</Header>

				<Content>
					<Text>This is body section</Text>
				</Content>
			</Container>
		);
	}
}
```

<div style="width:290px;height:593px;margin-left:auto;margin-right:auto;background-image:url(/images/iphone.png)">
		<iframe style="border-width:0px;background-color:white;
		width:337px;height:600px;margin-left:-23px;margin-top:-10px;
		-ms-transform: scale(0.75);
    -moz-transform: scale(0.75);
    -o-transform: scale(0.75);
    -webkit-transform: scale(0.75);
    transform: scale(0.75);
		" src="http://localhost:3000/#/app/2"></iframe>
</div>

## Content

* This is a NativeBase component which renders as body element of your screen.
* Each screen can have only one `<Content>` component and can be defined anywhere within the Container.
* Content takes in the whole collection of React Native and NativeBase components.
* Content provides you with stylesheet.
* User can add custom styles while defining `<Content>` within their app.
* Replacing Component: React Native `<ScrollView>`
