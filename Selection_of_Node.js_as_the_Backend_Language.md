# Architecture Decision Record for Scenario 2: Social Networking Mobile App
**Decision Title:** Selection of Node.js as the Backend Language
**Date:** Oct 5, 2023
**Team members:** Matthew Yackel, Duc Nguyen

## Background
In the process of making architectural decisions for our university social networking mobile app, we need to choose the appropriate backend language. This decision will significantly impact how we handle data, authentication, and overall application performance. Our goal is to select a backend language that aligns with our project's objectives and requirements.

**Decision:** We have decided to use Node.js as the backend language for the university social networking mobile app.

## Rationale:
The decision to select Node.js as the backend language is based on the following key reasons:

- **JavaScript Synergy:** Since we are already using JavaScript with React Native for the frontend, choosing Node.js for the backend allows for code and library sharing between the frontend and backend, streamlining development and reducing potential inconsistencies.

- **JWT Authentication:** Node.js is well-suited for implementing JWT (JSON Web Tokens) for authentication and authorization, ensuring secure user access control to the app's features and data.

- **Firebase Integration:** Node.js seamlessly integrates with Firebase databases, which offer robust support for various authentication methods, including email/password, phone number, and social sign-in. This integration enhances our ability to manage user data securely and efficiently.

## Consequences:
While Node.js offers numerous advantages, there are also potential consequences to consider:

- **Learning Curve:** If team members are not already familiar with Node.js, there may be a learning curve, although this is mitigated by the shared JavaScript expertise.

## Conclusion:
By selecting Node.js as our backend language, we aim to ensure a cohesive and efficient development process, enabling secure authentication, data management, and seamless integration with other components of the app. The scalability and compatibility with Firebase make it a solid choice for handling sensitive user data and ensuring data privacy and security.
