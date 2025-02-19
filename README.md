# MemoMind README

## Introduction
MemoMind is a note-taking app aiming to help make users more productive in note-taking with its simplistic use for organization and customization.

## Components

### Backend
<!-- mention API's present and how they could be triggered? > -->
#### Backend Overview
The backend is built on Node.js and Express, designed to handle web requests and interact with a MongoDB database. It uses several npm packages such as express, mongoose, cors, express-session, and bcrypt for various functionalities. The backend is connected to MongoDB to store and manage application data. The connection string and database name are specified, and the connection is established using the MongoDB client. 

We chose to use MongoDB for this application due to its flexibility in handling diverse data types and structures, enabling dynamic content management with ease. Its schema-less nature allows for rapid development and iteration, accommodating changes in data structure without significant overhead. Additionally, MongoDB's powerful query language and scalability make it ideal for managing large volumes of data, ensuring the application can grow and adapt to user needs efficiently.

#### API Endpoints
The application defines several API endpoints grouped by functionality, such as user authentication, profiles, notes, events, friend management, and more. These endpoints allow the frontend application to perform operations like login, signup, profile update, notes management, event scheduling, and handling friend requests.
*User Authentication (/api/login, /api/signup): Allows users to login and signup. Passwords are hashed using bcrypt for secure storage.

* Profile Management (/api/profile): Enables fetching and updating user profiles.

* Notes Management (/Notes): Allows users to create, update, fetch, and delete notes.

* Event Management (/api/events): Enables users to add, fetch, and delete calendar events.

* Friend Management (/FriendManager): Handles sending, accepting, and removing friend requests, as well as managing friends list and friend requests.

* Privacy Management (/PrivacyManager): Allows users to update the privacy settings of their notes.

#### Triggering  API Endpoints
The API endpoints can be triggered by making HTTP requests (GET, POST, PUT, DELETE) from any frontend application Each endpoint has a specific route (e.g., /api/login, /Notes) and expects certain request parameters or body content. For example, the login endpoint expects a POST request with an email and password in the request body.

### Frontend
The frontend of the application is designed as a comprehensive and interactive platform, developed using React for dynamic user interfaces. It incorporates a variety of components for different functionalities, including Calendar, Friend Manager, Images, Layout, LoginSignup, NotesApp, PrivacyManager, Profile, and Videos, each managed by a dedicated CSS file for styling. Navigation between these components is facilitated by React Router, ensuring a seamless and secure user experience with protected routes for authenticated access only.

The Layout component wraps around the main content, providing a consistent structure across the app with a navigation sidebar that offers quick access to all main features like notes, calendar, images, videos, profile management, privacy settings, and friend management. It also features a logout button and displays the user's name, enhancing the personalized experience.

This frontend setup aims to provide an intuitive, user-friendly interface, allowing users to efficiently manage their personal information, appointments, and social interactions within a single application.

### Datastore
The datastore for this application is implemented using MongoDB, which is flexible, scalable, and enables the handling diverse data structures. It storings and managing a wide array of data types across various collections, including users, profiles, notes, events, images, videos, and friend relationships. This choice allows for efficient storage and retrieval of dynamic content, user authentication details, personal media, calendar events, and social interactions, catering to the application's complex data handling needs. MongoDB's schema-less nature significantly aids in rapid development and iteration, enabling the application to evolve seamlessly as requirements grow or change.

## Setup
### Option 1: Setup With setup.sh
1. Clone the repository 
`$ git clone https://github.com/cindydingg/MemoMind`
or download the zip on GitHub.

2. Make sure you're in the directory
`$ cd MemoMind`

3.  Make setup.sh executable
`$ chmod +x setup.sh`

4. Run setup.sh to install dependencies and run project!
`$ ./setup.sh`

5. Play around!
Create an account and have fun, the content will be saved for your account.

### Option 2: Setup With Commands
1. Clone the repository 
`$ git clone https://github.com/cindydingg/MemoMind`
or download the zip on GitHub.

2. Make sure you're in the directory
`$ cd MemoMind`

3.  Install npm
`$ npm install`

4. Start the app!
`$ npm run dev`

5. Play around!
Create an account and have fun, the content will be saved for your account.


## Commands
`$ git clone https://github.com/cindydingg/MemoMind`

`$ cd MemoMind`

`$ npm install`

If run into issue with `Error: Can't resolve 'draft-js-plugins/editor'` try: `$ npm install @draft-js-plugins/editor`

`$ npm run dev`

## Contributors
* Cindy Ding (cindydingg): contributed to image upload, video upload, notes page
* Sharon Chen (sharonc05): contributed to login/signup, calendar, calendar events, labels, navigation bar
* Jermaine Xie (JJjermaine): contributed to login/signup, notes page, MongoDB setup, friend management, notes privacy 
* Albert Le (albert97567): contributed to login/signup page, MongoDB setup, password encryption, notes searchbar, labels searchbar

## Examples of How Project Should Behave
### Signing Up and Logging In
https://github.com/user-attachments/assets/f6889e95-2efb-4e29-b2fe-c08bc7a5e915

### Making Notes
https://github.com/user-attachments/assets/c70a9dd0-e5d3-4698-909b-137f07ebb572

### Editing Notes, Adding Labels
https://github.com/user-attachments/assets/4fa2b9fa-eb1f-416b-8722-8d3db40b5029

### Searching Through Notes
https://github.com/user-attachments/assets/45912b4c-4325-4f7e-80f8-f4ba296d2b03

### Calendar and Events
https://github.com/user-attachments/assets/4f6c56a8-113c-4dc2-884a-c3a22c9817c9

### Adding Images
https://github.com/user-attachments/assets/535e0d05-b7b8-4bea-998f-789c3ab3354e

### Adding Videos
https://github.com/user-attachments/assets/d00eaacf-3664-4bb5-bfc0-e0b5d2890fbb

### Viewing Profile
<img width="1502" alt="viewing-profile" src="https://github.com/user-attachments/assets/a6c90fcb-7c1e-47ff-8478-0b70e29d0033">

### Managing Notes Privacy
https://github.com/user-attachments/assets/473d585a-7d6a-48ce-a88c-21421825f3b0

### Requesting Friends
https://github.com/user-attachments/assets/68701a18-e787-495e-9c40-d47daf9a2d73

### Accepting Friends
https://github.com/user-attachments/assets/ee3b9a51-67d6-42ac-b123-7ba33c499ecc

### Viewing Friend's Notes
https://github.com/user-attachments/assets/0768e747-7a62-48e5-8b18-d66a7029d0c2
