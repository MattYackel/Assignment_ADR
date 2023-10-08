# Architecture Decision Record for Scenario 2: Social Networking Mobile App
**Decision Title:** Choice of Local and Remote Storage
**Date:** Oct 8, 2023
**Team members:** Matthew Yackel, Duc Nguyen

## Background
Students and professors may not always have access to a stable internet connection. Support for an offline mode would enable users to continue to use some features of the app regardless of connectivity. 

## Decision
Our team has decided to implement an offline mode with local caching and local queing for data, as well as data synchronization to sync the local changes to the MongoDB database when there is a network connection available. This can be done using a synchronization data approach, where data will be stored locally in the device's cache or local queing to store the data in non-volitile memory. When a network connection is re-established, the data will be sent to the database server to synchronize the data. 

## Reasoning 
Implementing an offline mode feature with MongoDB is the most suitable choice for this scenario for several reasons: 
- **MongoDB Local and Remote Storage:** MongoDB provides support for using local storage as well as synchronizing it with a server. 
- **Node.js Backend Logic:** Since we are using Node.js for the backend of the project, we can use it to create customized syncronization logic for conditions on when to use local storage, and when to queue and sync data to the server. 
- **Offline Functionality:** Using local storage as temporary storage will enable the offline mode functionality for when a network connection is not available, or when the network connection is unreliable. 
- **Network Optimization and Reliance:** By supporting local caching and offline functionality, there is less reliance on having a stable network connection to use the app, preventing data loss and service interruptions. This will also reduce the amount of network usage by sending data to the database less often and in larger chunks, rather than frequent small requests. 

## Consequences
While there are clear advantages with supporting an offline mode, there are also negative implications that must also be considered: 
- **Offline Mode Development:** Adding an offline mode is a large funtion. This will require more development time to implement. 
- **Learning Curve:** While the team is familiar with MongoDB and Node.js, working with local and network storage and connectivity in a database is a new concept which must be researched. This will result in more development time due to learning and troubleshooting. 

## Conclusion
Implementing a synchronization data aproach to enable an offline mode for the app will allow a smooth user experience regardless of internet connection and network reliability. This will also allow us to reduce network usage and reliance. 