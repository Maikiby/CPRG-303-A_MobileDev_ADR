# Architectural Decision Record for Scenario 2

Written by Sergio Martinez
For the CPRG 303 Block A Class

## Top-level

* Title
* Native, web, or hybrid app
* UI Framework
* Backend language
* Permissions
* Data storage
* Miscellaneous

## Low-level deep dive

**Title**:

  * Architectural Decision Record for Scenario 2

**Native, web, or hybrid app**:

  * The app would be a Hybrid app, as it would be a mobile app that needs to be able to run on both Android and iOS devices.

**UI Framework**:

  * The Framework to be used is React Native, as it allows for the app to run on both Android and iOS. It is also a Framework we are familiar with, and it is easy to learn.

**Backend language**:

  * ExpressJS could be used to to handle the backend of the app. It is a lightweight framework that is easy to use, and it is ideal for small apps.

**Permissions**:

  * The app will integrate with Active Directory and provide a login screen for users to login with their credentials. After which, it will provide access to specific features based on the user's role.

**Data storage**:

  * Firebase was chosen because it is a NoSQL database, and it is easy to use. It is scalable, and ideal for proof-of-concept apps. We can also migrate to MongoDB if we need to take the app to production. 
  * Critical and confidential data will be encrypted to ensure user privacy and security.

**Miscellaneous**: 
  * Since we're already using Firebase as the Database, we can use Firebase Cloud Messaging in order to manage push notifications in the app. 
  * The app would use multi-factor authentication to ensure user security. Ideally, we would make use of passkeys, biometrics, and/or facial recognition.
  * The app would be able to run offline, and sync with the database when the user is online. We would minimize the amount of data stored on the device by caching it regularly and only storing the most recent data.