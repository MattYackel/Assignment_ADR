# Architecture Decision Record for Scenario 2: Social Networking Mobile App
**Decision Title:** Choice of Permissions and Access Control
**Date:** Oct 7, 2023
**Team members:** Matthew Yackel, Duc Nguyen

## Background
Since the app is intended to be used only by students or instructors currently attending the university, our team needs to implement a solution to enforce permissions and control access rights for users. The app will also be dealing with sensitive user information, so having a secure and robust authentication system is crucial. 
## Decision
Our team has agreed that the best approach to securing app permissions and access control is to incorporate the app with the university's existing Active Directory system for user authentication. This system can be used to facilitate secure login, roles, and permissions for users as a role-based access control (RBAC). User roles and permissions would be consistent and dynamic with the university, so only current students or instructors would have access to the app. 
## Reasoning 
The decision to use the usinversity's AD system to handle to app's permissions and access control is based on the following key reasons:
- **Enhanced Security:** Using the existing AD system is the best approach to enforcing user security because this will ensure that only currently active university students or intructors will have access to to app. Otherwise preventing users who are not a current student or instructor would be more difficult to develop, update, and enforce. 
- **Using an Existing System:** Using an existing Active Directory database will reduce development time by not having to develop a new access control system. Any changes to the university's system will also be applied dynamically and automatically to the permissions used on the app. 
## Consequences
While using the existing AD system has advantages, there are also negative consequences attributed to the approach. 
- **Learning Curve:** Connecting an app to an Active Directory database is new to our team, so there will be a learning curve when developing the authentication for the app. Because of this, more time will be required for development. 
- **Reliance on External System:** By using an existing system for authentication and permissions, the app will be reliant on that system being online and for data to be accurate. Any service interruptions on the AD system could also interrupt our app. This would also result in more reliance on having a network connection, as well as increasing network usage. 
## Conclusion
Our team will enforce permissions and access controls by using the existing university's Active Directory system for user authentication, permissions, and roles within our app. This approach will result in accurate and dynamic user authentication verification. 