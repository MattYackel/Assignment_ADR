# Architecture Decision Record for Scenario 2: Social Networking Mobile App
**Decision Title:** Choice of Encryption
**Date:** Oct 6, 2023
**Team members:** Matthew Yackel, Duc Nguyen

## Background
Since the app will be dealing with sensitive user information such as student grades and profile information, our team has been researching different data encryption methods. This sensitive data must be protected where the data is stored locally and on the database, as well as when it is transmitted over the network. 

## Decision
Our team has decided to incorporate data encryption with MongoDB's transparent data encryption (TDE) feature. 

## Reasoning 
The decision to use MongoDB's TDE for data encryption is based on the following key reasons:
- **Enhanced Security:** Using MongoDB for encryption will keep local data secure in addition to the remote database, both of which are used to enable the offline-mode functionality. Having sensitive data encrypted in addition to the authentication restricted using the university's Active Directory system will provide multiple layers of security to make sure the data i sonly available to it's intended user. 
- **Development Impact:** Our team agrees that implementing encryption at rest with MongoDB for data such as student grades and personal profile data will be the best approach to ensure data privacy and security within the app. MongoDB's TDE is simple to implement. 
- **Minimal Performance Impact:** MongoDB's TDE is a built-in feature, and is designed to have a minimal impact on performance. 

## Consequences
While encryption with MongoDB offers numerous advantages, there are also potential consequences to consider:
- **Learning Curve:** Data encryption in MongoDB is new to our team, so there will be a learning curve when applying data encryption. Because of this, more time will be required for development. 
- **Performance Impact:** Although minor, adding extra steps to provide data encryption will inevitably impact performance. 

## Conclusion
Our team will provide data encryption in MongoDB using transparent data encryption (TDE) for sensitive data such as student grades and user profile information. This will ensure that data privacy and security remains a priority for the app. 