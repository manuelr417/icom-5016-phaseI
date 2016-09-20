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
3. **Controller** - the layer that implements the control logic to route the requests from the UI to the objects in the Model that implement the necessary logic of the application. This layer is implemented with Node.js, Java Play, or Pythin Flask. In Phase I, you implement very basic versions of controller which simply respond inmediately to the UI with an OK response.  

### REST API
Your application's UI must communicate with the controller via a [REST api] (http://www.restapitutorial.com). REST is a method in which your application requests access to data and server-side operation by issuing an HTTP request as if it would be requesting a web page. For example, say an app name *myuber* need to find the location of car *c3272*, and suppose the backend has address myber.com. Then the UI will issue a request as : `http://myuber.com/findcar/c3272`. In this case, *findcar* is the operation we want to make and c3272 is the parameter. You can implement your entire app using this scheme. In fact, you can support different UI since REST is supported by Android, iOS, Javascript and many other UI frameworks. 

The response of the server comes encoded in JSON (Javascript Object Notation) which is supported by Android, iOS, Javascript, etc. For example, the response from the backend to the request the we mentioned above could be encoded as follows:
```
{
  'Car' : 'c3272',
  'Latitute': 18.4393,
  'Longitude': 64.484,
  'Time' : '12:04 PM',
  'Day' : '09/09/2016'
}
```
### Deliverables

Submit a Github repository with al the code, plus the report for Phase I. A template for the report can be found in this repo. **You application must run and be demostrable**. Your github repo might simply have two folders: 1) the client project and 2) the server project. Or, you can have everyhting integrated, particularly if your have a web application.

## Bonus points
Your project need to run locally on your laptop, perhaps using Eclipse, NetBeans, or InteliJ. *Up to 10 bonus points can be earned for phase I if your project runs on a real server (e.g., Amazon, Heroku) and an a real device (e.g., android phone.* 

## Due Date: 11:59 pm, October 12, 2016 



