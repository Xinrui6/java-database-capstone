## Architecture summary
The spring boot application uses both RESTcontrollers and MVC controllers. Thymeleaf templates are used for the Admin and Doctor dashboards. The other modules are served by REST APIs. The application interacts with two databases: a structured database MySQL for data of admin, doctor, patients, and appointments. Other data such as prescriptions interact with an unstructured database MongoDB. All controllers work through the common service layer, turn to the appropriate repositories, MySQL repositories, which using Spring Data JPA to manage structured relational data, or MongoDB Repository which uses Spring Data Mongo DB to manage document-based records.

## Numbered flow of data and control
1. User accesses AdminDashboard DoctorDashboard or Appointment, PatientDashboard or PatientRecord page. 
2. The HTTP request arrives at the Controller Layer, and routes it to the appropriate controller method for handling, Thymeleaf Controllers or REST Controllers.
3. The controller calls the service layer, exucuting all business rules and complex validations, and involve in multiple data entities.
4. Use MySQL repository or MongoDB Repository to access database and retrive or persistthe data, such as booking appointment, get the presciption, etc.
5. The  The repository layer will translate the method into database commands and interacts with the database by JPA to generate SQL to excuted in the MySQL, and MongoDB repository to excuted in the MogoDB database.
6. the framework will binds to hava object models. Data from MySQL wil converted into JPA entity objects. MongoDB collections will be converted into document objects
7. And the response will be generated and take the data back to the web requests through Thymeleaf template engine or as JSON string to the API requests.
