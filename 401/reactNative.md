# Reading

### [getting started with react native](https://facebook.github.io/react-native/docs/getting-started)

1. Three core components of React Native are:
   - **View**: View is like the `<div>` element in web development. It is a container that helps to group and layout other components. It is used to create the structure of the user interface.
   - **Text**: Text is used to display text content in a React Native app. It is similar to the `<p>` or `<span>` elements in web development. Text supports basic styling and text formatting.
   - **Image**: Image is used to display images in a React Native app. It is similar to the `<img>` element in web development. It supports various image sources, resizing, and other image-related features.

2. React Native solves the problem of building mobile applications that can run natively on multiple platforms (such as iOS and Android) using a single codebase. It allows developers to write code in JavaScript and use React-like components to create a user interface that is rendered as native components on the target platforms. This approach provides the benefits of code reuse, faster development cycles, and the ability to leverage platform-specific features, resulting in a more efficient and productive development process.

3. The building blocks of a React Native app include:
   - **Components**: React Native provides a set of pre-built UI components that can be combined to create the app's user interface. These components are similar to the building blocks in a React app.
   - **APIs**: React Native exposes a set of APIs that allow developers to interact with native platform functionalities, such as accessing the device's camera or reading location data. These APIs are different from a React app because they provide access to platform-specific features.
   - **Styling**: React Native uses a similar styling approach as web development, where styles are defined using CSS-like properties. However, React Native uses a different set of properties tailored for mobile platforms.

### [expo](https://expo.io/)

1. Expo provides a comprehensive development environment and platform for building mobile applications using React Native. It offers a range of tools, services, and libraries that simplify and streamline the app development process.

2. Expo tries to manage as much of the complexity of building apps as possible, which is why we call it the "Managed" workflow. In the Managed workflow, Expo takes care of many common tasks such as building, deploying, and updating the app, managing dependencies, providing access to native APIs, and handling platform-specific configurations. This allows developers to focus on writing the app logic and user interface without getting overwhelmed by the intricacies of the underlying platform.

3. The main difference between React Native and Expo is that React Native is a framework and runtime for building native mobile applications, while Expo is a set of tools and services built around React Native to simplify the development process. React Native provides the core runtime and libraries, whereas Expo builds on top of React Native and offers additional features like a development server, build infrastructure, push notifications, over-the-air updates, and access to native APIs through a unified interface. Expo can be seen as an extension of React Native that provides a higher-level abstraction and a more streamlined development workflow.

### [expo snack](https://snack.expo.io/)

1. Expo Snack is an online platform that allows developers to experiment, test, and build React Native apps directly from the browser. It provides an in-browser development environment with a code editor and a live preview of the app. Developers can write React Native code, import libraries, and see the app's output in real-time without the need to set up a local development environment.

### [ejecting](https://docs.expo.io/versions/latest/expokit/eject)

1. "Eject" in the context of Expo refers to the process of transitioning an Expo-managed project to a bare React Native project. When you eject, you essentially detach your project from Expo's managed workflow and gain more control over the underlying native code and configurations. Ejecting allows you to customize your project's native code, add native modules, use custom build configurations, and have more direct access to the platform-specific features.

2. You should not eject if you don't have a specific need for modifying the native code or if you want to continue using Expo's managed workflow. Ejecting adds complexity to the development process and requires you to take on the responsibility of maintaining the native code, including handling updates, building the app, and dealing with platform-specific configurations. If you're satisfied with the features provided by Expo and don't have requirements that necessitate ejecting, it's generally recommended to stick with the managed workflow.

3. You might choose to eject from Expo for several reasons:
   - **Custom Native Modules**: If you need to use a native module that is not available through Expo's APIs, ejecting allows you to add custom native code and integrate those modules into your project.
   - **Fine-grained Control**: Ejecting gives you more control over the native code, configurations, and build process, allowing you to tailor your app to specific requirements.
   - **Third-Party Libraries**: If you need to use third-party libraries that require custom native code modifications, ejecting enables you to integrate them into your project.
   - **Platform-specific Features**: Ejecting allows you to access and leverage platform-specific features and APIs that are not yet supported or exposed through Expo.

## Tutorial

### [react native basics](https://facebook.github.io/react-native/docs/tutorial)

The "React Native Basics" tutorial provides a step-by-step guide to building a simple React Native app. It covers topics such as setting up a development environment, creating components, handling user input, styling components, and navigating between screens. The tutorial is a great starting point for beginners who want to get hands-on experience with React Native development.

## Bookmark and Review

[react native](https://facebook.github.io/react-native/)

## [Back](../401readingNotes.md)