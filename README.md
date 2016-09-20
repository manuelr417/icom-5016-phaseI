# ICOM 5016 Fall 2016
## Project Phase I
## Due Date: 11:59 pm, October 12, 2016 
### Introduction
In Phase I of the project you will work with the User Interface (UI) design and ER model of the application. In particular, you will:

1. Implement the UI of the application, whether it is a web-based application (regular o mobile), or an android-based application. 
2. Implement a basic backend.  Your UI will communicate with the backend server component, but no real data or connection to the database is required. Instead, the backend component always return the same dummy data to the UI. 
3. Develop an Entity Relationship (ER) diagram specifying the entities and relationships in use. 

Thus, as you can see, in Phase I your application is "hardwired" with dummy data, and you are only working to develop the workflow of screens from login (or registration) to using the features of your app.

### Organization of the Application
You application needs to be logically organized along the three layers of the **Model-View-Controller** (MVC) pattern:

1. **Model** - the layer that manages the business logic and storage of the application, including the communication with the DBMS. In this phase I you do not work with the model yet. This layer is implemented with a DBMS, SQL, and Objects (e.g., Plain Old Java Objects (POJOS), or Python objects). 
2. **View** - the layer that implement the UI of the application. This layer is the main focus of Phase I. This layer is implemented with things like HTML, CSS, JavaScript, Angular JS, etc. 
3. **Controller** - the layer that implements the control logic to route the requests from the UI to the objects in the Model that implement the necessary logic of the application. In Phase I, you implement very basic versions of controller which simply respond inmediately to the UI with an OK response. 


