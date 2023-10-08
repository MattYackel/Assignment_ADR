# Architecture Decision Record for Scenario 2: Social Networking Mobile App
**Decision Title:** Selection of Hybrid App Development
**Date:** Oct 5, 2023
**Team members:** Matthew Yackel, Duc Nguyen

## Background
In the process of deciding the architecture for our university social networking mobile app, we considered various approaches, including native, web, and hybrid development. Our goal is to choose an architecture that ensures widespread adoption, cross-platform compatibility, and efficient development while addressing the unique requirements of our app.

## Decision:
We have decided to develop the university social networking mobile app as a hybrid app.

## Rationale:
Developing a hybrid app is the most suitable choice for this scenario for several reasons:
- **Cross-Platform Compatibility:** The app's requirement to support both iOS and Android platforms can be efficiently met with a hybrid approach. A single codebase can be used to target multiple platforms, reducing development effort and time.
- **Efficient Development and Maintenance:** A hybrid app allows for efficient development and maintenance as updates and bug fixes can be applied uniformly across both platforms, reducing the development team's workload.
- **Access to Native Features:** Hybrid frameworks like React Native provide access to native device features and plugins, ensuring that the app can utilize device-specific functionality when necessary.

## Consequences:
- **Platform-Specific Challenges:** While hybrid apps provide access to native features, there may still be some platform-specific challenges or limitations that need to be addressed during development.

## Conclusion:
By choosing a hybrid app development approach, we can efficiently meet the app's platform requirements while optimizing development resources and ensuring a consistent user experience. The benefits of code reusability and efficient development outweigh the potential challenges associated with platform-specific issues.
