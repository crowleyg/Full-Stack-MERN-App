# Full Stack MERN App - Exercise Tracker App

This repository contains the code for an Exercise Tracker App, which allows users to store, manage, and track exercise data. The app includes a React-based user interface (UI) that communicates with a RESTful API and stores data in a MongoDB database.

## Table of Contents
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Getting Started](#getting-started)
- [REST API](#rest-api)
- [React UI](#react-ui)

## Features
The Exercise Tracker App offers the following features:

- Storing exercise data in a MongoDB collection named "exercises."
- Supporting CRUD operations via a REST API.
- Home Page to display all exercises in an HTML table with icons for editing and deleting.
- Edit Exercise Page for editing specific exercises with pre-populated data.
- Create Exercise Page for adding new exercises.
- Global navigation for easy access to different pages.

## Technologies Used
- MongoDB: A NoSQL database used to store exercise data.
- Express.js: A web application framework for building the REST API.
- React: A JavaScript library for building user interfaces.
- React Icons: A library providing icons for UI elements.
- Node.js: A JavaScript runtime used for server-side scripting.
- HTML5/CSS3: Markup and styling for the user interface.

## Getting Started
To get started with the Exercise Tracker App, follow these steps:

1. Clone this repository to your local machine.
2. Install Node.js and npm if not already installed.
3. Navigate to the project directory and install the required dependencies using `npm install`.
4. Set up your MongoDB database and update the database connection details in the API code.
5. Start the server and the React app using `npm start`.

## REST API
The app's REST API supports CRUD operations through the following endpoints:

1. **Create**: `POST /exercises`
   - Request: JSON object with exercise properties.
   - Response: JSON object with exercise properties and generated ID.
   - Status code: 201

2. **Read**: `GET /exercises`
   - Request: None
   - Response: JSON array containing all exercises with IDs.
   - Status code: 200

3. **Update**: `PUT /exercises/:id`
   - Request: JSON object with exercise properties.
   - Response: JSON object with updated exercise properties and ID.
   - Status code: 200

4. **Delete**: `DELETE /exercises/:id`
   - Request: None
   - Response: No response body.
   - Status code: 204

## React UI
The React-based user interface consists of three pages:

### Home Page
- Displays all exercises in an HTML table.
- Allows users to delete exercises and navigate to the Edit Exercise Page.
- Provides a link to the Create Exercise Page.

### Edit Exercise Page
- Allows users to edit exercise details.
- Pre-populates controls with existing exercise data.
- Provides a button to save updates, show success alert, and return to the Home Page.

### Create Exercise Page
- Enables users to add new exercises.
- Includes input controls for exercise properties.
- Provides a button to save new exercise, show success alert, and return to the Home Page.
