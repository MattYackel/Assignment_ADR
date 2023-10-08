# Architecture Decision Record for Scenario 2: Social Networking Mobile App
**Decision Title:** Selection of React Native as the UI Framework
**Date:** Oct 5, 2023
**Team members:** Matthew Yackel, Duc Nguyen

## Background
In the process of making architectural decisions for our university social networking mobile app, we need to select the appropriate UI framework. This decision will significantly impact the development process and the user experience. Our goal is to choose a UI framework that aligns with our project's objectives and requirements.

**Decision:** We have decided to use React Native as the UI framework for developing the university social networking mobile app.

## Rationale:
The decision to select React Native as the UI framework is based on the following key reasons:
- **JavaScript and React Expertise:** React Native leverages JavaScript and React, which are widely used technologies with a large developer community. Since the team is already familiar with JavaScript and React, this choice minimizes the learning curve and accelerates development.
- **Cross-Platform Compatibility:** React Native is renowned for its cross-platform compatibility, allowing developers to write code once and deploy it on multiple platforms, aligning with the requirement to support both iOS and Android.
- **Abundance of Libraries:** The React Native ecosystem boasts a vast array of open-source libraries and UI component libraries that can expedite development and enhance the app's functionality. This rich ecosystem is a valuable resource for creating features like social networking and event management.

## Consequences:
While React Native offers numerous advantages, there are also potential consequences to consider:
- **Platform-Specific Challenges:** Although React Native provides access to many native device features, there may be cases where custom native modules are required. This can introduce additional complexity to the development process.

## Conclusion:
By choosing React Native as our UI framework, we aim to maximize development efficiency, maintain code quality, and leverage a robust ecosystem of tools and libraries. The advantages of rapid development and cross-platform compatibility make React Native an excellent fit for this project, despite the potential platform-specific challenges that may arise.
