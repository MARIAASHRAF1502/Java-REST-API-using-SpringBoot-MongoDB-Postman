
## How to Run this project locally on your machine ?


![clone0](https://github.com/MARIAASHRAF1502/Java-REST-API-using-SpringBoot-MongoDB-Postman/assets/67148270/73072309-bd11-4057-aff4-ceeebd7a127d)
![clone1](https://github.com/MARIAASHRAF1502/Java-REST-API-using-SpringBoot-MongoDB-Postman/assets/67148270/63acf951-dd6a-4e00-8e55-2c6fbed5df57)


- Open Spring Boot IDE and navigate to windows -> show view -> other -> Git -> Git Repositories and click Open.
![clone2](https://github.com/MARIAASHRAF1502/Java-REST-API-using-SpringBoot-MongoDB-Postman/assets/67148270/035b0c10-4533-4d66-a536-6bb0c8e686a2)
![clone3](https://github.com/MARIAASHRAF1502/Java-REST-API-using-SpringBoot-MongoDB-Postman/assets/67148270/33ca552d-b4ef-4b43-be70-3074177b8c42)

- In the wizard, paste the following respository "https://github.com/MARIAASHRAF1502/Java-REST-API-using-SpringBoot-MongoDB-Postman.git" in the URI Text field. 
- Click Next -> choose the Branch as "Master" -> Finish.


![clone4](https://github.com/MARIAASHRAF1502/Java-REST-API-using-SpringBoot-MongoDB-Postman/assets/67148270/bf9bc86a-eef2-47fd-9348-54f35e6e934f)
- From the "Git Repository Dashboard", Right click on the project folder and choose "Import projects".
- Now the project folder will be created on the  "Package Explore r" Dashboard to manipulate the files. 

## To Start the Server
![run](https://github.com/MARIAASHRAF1502/Java-REST-API-using-SpringBoot-MongoDB-Postman/assets/67148270/11f030ea-5648-4e42-bddc-209275304c70)

- From "Boot Dashboard" -> choose the project -> click on to the start project icon.
- If the port number is displayed next to the project name, then the server is Running successfully.

## Working of APIs

- Open Postman create a new Collection, Once the collection is created click on the 3 dots which is next to the Collection name,  and click "Add Request" for each Operations.

## Create Operation 


![create](https://github.com/MARIAASHRAF1502/Java-REST-API-using-SpringBoot-MongoDB-Postman/assets/67148270/7a3aba08-182f-468f-87a5-1dcf91d130b9)

- Set method as "POST" -> and enter the following the Address "http://localhost:8080/create"
- Click Body -> choose "raw" -> and format as "JSON", and enter the data in a JSON format as shown in above figure and click "Send".

## ReadAll Operation


![readAll](https://github.com/MARIAASHRAF1502/Java-REST-API-using-SpringBoot-MongoDB-Postman/assets/67148270/2d0fc0ec-9399-4bc5-a103-be21e97b4fe8)

- Set method as "GET" -> and enter the following the Address "http://localhost:8080/getServer".
- Click on Send to send the Request. And the response will be display in the response body section.

## Read Operation

![readbyId](https://github.com/MARIAASHRAF1502/Java-REST-API-using-SpringBoot-MongoDB-Postman/assets/67148270/32b5b96c-50c7-49d9-bb23-290230cd67e6)

- Set method as "GET" -> and enter the following the Address "http://localhost:8080/getServer/{serverId}". Pass the unique Sever Id along with the Address.
- If the server data exists in the database for the mentioned Server ID, it will fetch those records, otherwise it will display a 404 status code indicating 'No Data Found'.


![readbyId](https://github.com/MARIAASHRAF1502/Java-REST-API-using-SpringBoot-MongoDB-Postman/assets/67148270/48080b69-0737-4d7d-8179-50100ce41886)


## Delete Operation

![delete](https://github.com/MARIAASHRAF1502/Java-REST-API-using-SpringBoot-MongoDB-Postman/assets/67148270/49d58081-f541-4323-ac24-b10412457aac)

- Set method as "DELETE" -> and enter the following the Address "http://localhost:8080/deleteRecord/{serverId}". Pass the unique Sever Id along with the Address.
- If the server data exists in the database for the mentioned Server ID, it will delete those records, otherwise it will display a 404 status code indicating 'No Record Exist'.


![delete](https://github.com/MARIAASHRAF1502/Java-REST-API-using-SpringBoot-MongoDB-Postman/assets/67148270/bcd6f924-9444-4cf6-8963-bd41fd64a46e)

## Search Operation

![find](https://github.com/MARIAASHRAF1502/Java-REST-API-using-SpringBoot-MongoDB-Postman/assets/67148270/c837bdb7-8059-4822-a7b0-8e02fd5765ab)

- Set method as "GET" -> and enter the following the Address "http://localhost:8080/findRecord/{ServerName}". Pass the Sever Name along with the Address -> click send.
- If the server data exists in the database for the mentioned Server Name, it will fetch all the matching records, otherwise it will display a 404 status code indicating 'No Record Exist'.


![find](https://github.com/MARIAASHRAF1502/Java-REST-API-using-SpringBoot-MongoDB-Postman/assets/67148270/c6cf0864-8c0a-40d0-952f-c15c8fbbfe3f)











