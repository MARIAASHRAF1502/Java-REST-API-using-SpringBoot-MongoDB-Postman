
# Java REST API using Spring Boot, MongoDB and Postman

This project showcases the development of a robust REST API in Java. This API perform basic CRUD operation and manipulates the data stored in MongoDB database, by utilizing the powerful Spring Boot framework for efficient handling of HTTP requests.




## FAQ

#### What is REST API ?

REST API stands for Representational State Transfer Application Programming Interface. REST APIs are commonly used  to communicate data among client and server in a specified data format such as JSON, HTML, XML. REST API works on top of HTTP protocol to perform, GET (retrieve data), POST (create new data), PUT (update existing data), DELETE (remove data) operations efficiently in a Database.  In simple, it a light-weighted Architectural design for data inter-change.

#### What is Spring Boot ?

Spring Boot is a powerful Java-based framework that simplifies the process of building, deploying, and managing web applications. By utilizing Spring Boot, the developers can focus on business logic rather than boilerplate code. Spring Boot comes with pre-configured dependencies, making it simple to connect and communicate with various Databases. Spring Boot makes it easy to create RESTful APIs. Apache Tomcat is the default embedded server for Spring Boot. It's a widely used and well-established web server. It's simple to configure and provides good performance.

#### What is MongoDB ?

MongoDB is a NoSQL (Not Only SQL) database that offers a flexible, document-oriented approach to data storage. It stores data in JSON format, allowing for dynamic schema and easy scalability.

#### What is Postman ?

Postman is a widely-used and powerful API development and testing tool that simplifies the process of building, documenting, and testing APIs. Postman supports various request methods (GET, POST, PUT, DELETE, etc.) and allows for parameterization, authentication, and handling of headers. Postman helps in streamline the API development process.




## Installation

Software and tools required to work on this project are as follow

- JDK - https://www.oracle.com/in/java/technologies/downloads/

- Eclipse IDE - https://www.eclipse.org/downloads/packages/installer
- Spring Boot Tools for Eclipse - https://spring.io/tools
- MongoDb (Preferred version - 4 & above) - https://www.mongodb.com/try/download/community

- Postman - https://www.postman.com/downloads/


## How to Run this project locally on your machine ?


![clone0](https://github.com/MARIAASHRAF1502/Java-REST-API-using-SpringBoot-MongoDB-Postman/assets/67148270/73072309-bd11-4057-aff4-ceeebd7a127d)
![clone1](https://github.com/MARIAASHRAF1502/Java-REST-API-using-SpringBoot-MongoDB-Postman/assets/67148270/63acf951-dd6a-4e00-8e55-2c6fbed5df57)


- Open Spring Boot IDE and navigate to windows -> show view -> other -> Git -> Git Repositories and click Open.


![clone2](https://github.com/MARIAASHRAF1502/Java-REST-API-using-SpringBoot-MongoDB-Postman/assets/67148270/035b0c10-4533-4d66-a536-6bb0c8e686a2)
![clone3](https://github.com/MARIAASHRAF1502/Java-REST-API-using-SpringBoot-MongoDB-Postman/assets/67148270/33ca552d-b4ef-4b43-be70-3074177b8c42)

- In the wizard, paste the following respository "https://github.com/MARIAASHRAF1502/Java-REST-API-using-SpringBoot-MongoDB-Postman.git" in the URI Text field. 
- Click Next -> choose the Branch as "Master" -> click Finish.


![clone4](https://github.com/MARIAASHRAF1502/Java-REST-API-using-SpringBoot-MongoDB-Postman/assets/67148270/bf9bc86a-eef2-47fd-9348-54f35e6e934f)
- From the "Git Repository Dashboard", Right click on the project folder and choose "Import projects".
- Now the project folder will be created on the  "Package Explorer" Dashboard to manipulate the files. 

## To Start the Server
![run](https://github.com/MARIAASHRAF1502/Java-REST-API-using-SpringBoot-MongoDB-Postman/assets/67148270/11f030ea-5648-4e42-bddc-209275304c70)

- From "Boot Dashboard" -> choose the project -> click on to the start project icon.
- If the port number is displayed next to the project name, then the server is Running successfully.

## Working of APIs

- Open Postman create a new Collection, Once the collection is created click on the 3 dots which is next to the Collection name,  and click "Add Request" for each Operations.

## Create Operation 


![create](https://github.com/MARIAASHRAF1502/Java-REST-API-using-SpringBoot-MongoDB-Postman/assets/67148270/7a3aba08-182f-468f-87a5-1dcf91d130b9)

- Set method as "POST" -> and enter the following address 'http://localhost:8080/create'.
- Click Body -> choose "raw" -> and format as "JSON", and enter the data in a JSON format as shown in above figure and click 'Send'.

## ReadAll Operation


![readAll](https://github.com/MARIAASHRAF1502/Java-REST-API-using-SpringBoot-MongoDB-Postman/assets/67148270/2d0fc0ec-9399-4bc5-a103-be21e97b4fe8)

- Set method as "GET" -> and enter the following address "http://localhost:8080/getServer".
- Click on 'Send' to send the Request. And the response will be displayed in the response body section.

## Read Operation

![readbyId](https://github.com/MARIAASHRAF1502/Java-REST-API-using-SpringBoot-MongoDB-Postman/assets/67148270/32b5b96c-50c7-49d9-bb23-290230cd67e6)

- Set method as "GET" -> and enter the following address "http://localhost:8080/getServer/{serverId}". Pass the unique Sever Id along with the Address -> click send.
- If the server data exists in the database for the mentioned Server ID, it will fetch those records, otherwise it will display a 404 status code indicating 'No Data Found'.


![readbyId](https://github.com/MARIAASHRAF1502/Java-REST-API-using-SpringBoot-MongoDB-Postman/assets/67148270/48080b69-0737-4d7d-8179-50100ce41886)


## Delete Operation

![delete](https://github.com/MARIAASHRAF1502/Java-REST-API-using-SpringBoot-MongoDB-Postman/assets/67148270/49d58081-f541-4323-ac24-b10412457aac)

- Set method as "DELETE" -> and enter the following address "http://localhost:8080/deleteRecord/{serverId}". Pass the unique Sever Id along with the Address -> click send.
- If the server data exists in the database for the mentioned Server ID, it will delete those records, otherwise it will display a 404 status code indicating 'No Record Exist'.


![delete](https://github.com/MARIAASHRAF1502/Java-REST-API-using-SpringBoot-MongoDB-Postman/assets/67148270/bcd6f924-9444-4cf6-8963-bd41fd64a46e)

## Search Operation

![find](https://github.com/MARIAASHRAF1502/Java-REST-API-using-SpringBoot-MongoDB-Postman/assets/67148270/c837bdb7-8059-4822-a7b0-8e02fd5765ab)

- Set method as "GET" -> and enter the following address "http://localhost:8080/findRecord/{ServerName}". Pass the Server Name along with the Address -> click send.
- If the server data exists in the database for the mentioned Server Name, it will fetch all the matching records, otherwise it will display a 404 status code indicating 'No Record Exist'.


![find](https://github.com/MARIAASHRAF1502/Java-REST-API-using-SpringBoot-MongoDB-Postman/assets/67148270/c6cf0864-8c0a-40d0-952f-c15c8fbbfe3f)














## Code Explanation !

1.  _/src/main/resources/application.properties

```
server.port = 8080
spring.data.mongodb.uri = mongodb://localhost:27017/KaiburrServer

```
- Server Port Configuration: You can specify the port on which your application will run.
- Database Configuration: You can specify database connection properties like URL, Port number and Database in which the data needs to be stored.

2. _/src/main/java/com.example.demo/ServerDetails.java

```
package com.example.demo;

import org.springframework.data.mongodb.core.mapping.Document;
import org.springframework.data.annotation.Id;

//mentioning the collection name under the mentioned database...
@Document(collection = "ServerRecords")
public class ServerDetails {
	
	@Id
	private int id;
	private String name;
	private String language;
	private String framework;
	
	
	public int getId() {
		return id;
	}


	public void setId(int id) {
		this.id = id;
	}


	public String getName() {
		return name;
	}


	public void setName(String name) {
		this.name = name;
	}


	public String getLanguage() {
		return language;
	}


	public void setLanguage(String language) {
		this.language = language;
	}


	public String getFramework() {
		return framework;
	}


	public void setFramework(String framework) {
		this.framework = framework;
	}


	public ServerDetails(int id, String name, String language, String framework) {
		super();
		this.id = id;
		this.name = name;
		this.language = language;
		this.framework = framework;
	}

}

```
- This file represent the Schema of the Collection, in which the attributes are specified.
- Getter and Setter methods are used to access the identifers.
- @Document annotation are used to represent as a MongoDB entity.


3. _/src/main/java/com.example.demo/ServerRepository.java

```
package com.example.demo;

import java.util.List;

import org.springframework.data.mongodb.repository.MongoRepository;
import org.springframework.stereotype.Repository;


@Repository
public interface ServerRepository  extends MongoRepository<ServerDetails,Integer>{

	List<ServerDetails> findByName(String serverName);
	

}

```

- To facilitate CRUD Operations on the Collection 'ServerRepository' interface is created, which extends 'MongoRepository' class to Control GET, PUT, POST, DELETE Operations.
- findByName() method is not a pre-defined function, it is used to find the Records based on the Server Name.



4. _/src/main/java/com.example.demo/ServerController.java

```
//	Delete operation based on the Server Id and return 404 when data not found...
@DeleteMapping(value = "/deleteRecord/{serverId}")
public ResponseEntity<String> deleteServerRecord(@PathVariable Integer serverId) {
Optional<ServerDetails> data = serverRepository.findById(serverId);

if(data.isEmpty()) {
	return new ResponseEntity<>("Record Not Found",HttpStatus.NOT_FOUND);
}		

serverRepository.deleteById(serverId);
return new ResponseEntity<>("Record Deleted successfully",HttpStatus.OK); 
		
	}
```

- @DeleteMapping annotation is used to perform DELETE operation and it execute when '/deleteRecord/{serverId}' URI is encountered.
- @PathVariable is used to get the data from URI, based on the data first the available Record is fetched from the database, if no record is found return the HttpStatus code 404 because if no data exist then delete operations can't be performed, else perform delete Operation and return HttpStatus code 200.

```
// insert Operation...
@PostMapping(value = "/create")
	public ResponseEntity<String> createServerRecord(@RequestBody ServerDetails server) {
		ServerDetails insertedRecord = serverRepository.insert(server);		
		return new ResponseEntity<>("Server "+insertedRecord.getName().toUpperCase()+" details inserted in Mongodb Database successfully ",HttpStatus.CREATED);
	}

```
- @PostMapping annotation is used to perform POST operation and it execute when '/create' URI is encountered.
- @RequestBody is used to get the data from body of the payload, and insert those data into a database and return a HttpStatus code as 201.
## 

                                                                           Happy Learning !

