# React Native

*React Native* is an open-source UI software framework created by Meta Platforms, Inc. It is used to develop applications for Android, Android TV iOS, macOS, tvOS, Web, Windows and UWP by enabling developers to use the React framework along with native platform capabilities.It is used to develop the Android and iOS applications at Facebook, Microsoft, and Shopify.

## Name three Core Components of React Native and describe what they do.

**1-View**
component is like a container that's used to structure and group other UI elements. It's similar to the HTML`<div>` element and is often used to create layouts and arrange components on the screen.

**2-Text**
component is used to display text on the screen. It's similar to the HTML <p> or <span> elements and allows you to render text content with styles such as font size, color, and alignment.

**3-Image**
 component is used to display images on the screen. It allows you to load and display images from local sources or remote URLs. You can also apply styles to control the image's size and position.

**Code Example**

```JS
import React from 'react';
import {Text, View} from 'react-native';

const YourApp = () => {
  return (
    <View
      style={{
        flex: 1,
        justifyContent: 'center',
        alignItems: 'center',
      }}>
      <Text>Try editing me! 🎉</Text>
    </View>
  );
};

export default YourApp;
```


## What problem does React Native solve (why call it native)?
React Native solves the problem of cross-platform mobile app development. It allows developers to build mobile applications using a single codebase in JavaScript and React while achieving a native look and feel on both iOS and Android platforms. 

## What are the building blocks of a React Native app? How does that compare to a React app?
Building blocks of a React Native app include components like View, Text, and Image for UI, and it uses native modules for device-specific functionality. React Native apps share UI components but utilize native components for the actual rendering, unlike React apps that rely solely on web-based components for both UI and functionality.


## What solution does expo provide?
Expo provides a development framework and platform for simplifying the building and deployment of React Native apps. It offers tools, libraries, and services to streamline the development process, including a managed development environment, pre-built UI components, and simplified app distribution.


#### Expo tries to manage as much of the complexity of building apps as possible, which is why we call it the `Managed` workflow.


## What is the difference between React Native and Expo? 
**React Native**:
- More flexibility and control
- Manual native dependency management
- Suitable for extensive customization

**Expo**:
- Set of tools and services
- Simplified development
- Limited native module access
- Ideal for rapid prototyping and streamlined development

## Checkout this tool. What does snack allow you to do?
Snack allows you to edit React Native code online, see live previews on your phone, and generate shareable URLs for collaborative development and testing.

## What does “eject” mean within the context of Expo?

`Eject` in the context of Expo means transitioning from Expo's managed development environment to a standard React Native project, providing greater control and access to native modules.


## When should you not eject?

-  app doesn't require extensive native module usage.
-  need rapid prototyping or simple app development.
-  prefer a cross-platform, hassle-free development experience.
-  team lacks experience in native mobile app development.
-  want simplified app store deployment.



