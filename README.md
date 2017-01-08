#**Lab Microservices - Web Engineering 2016-2017**

##**Setup**
### Server Eureka is launched
![Server Eureka Terminal](images/TerminalRegister.png)



##**The two Microservices are running in the port 2222, 3333 and registered**
### Services Registration
![Server Eureka Account Microservice 1 Terminal](images/TerminalRegister1.png)
![Server Eureka WebService Microservice Terminal](images/TerminalRegister2.png)

### Account Microservice
![Account Microservice 1 Terminal](images/TerminalAccount1.png)
![Account Microservice 1 Browser](images/ServiceAccount1.png)

### WebService Microservice
![WebService Microservice Terminal](images/TerminalWeb.png)
![WebService Microservice Browser](images/ServiceWeb.png)



##**The service Registration Service Eureka has the two Microservices registered**
### Server Eureka
![Server Eureka 1 Browser](images/ServiceRegister1.png)



##**Second Account Microservice is running in the port 4444 and it is registered**
### Service Registration
![Server Eureka Account Microservice 2 Terminal](images/TerminalRegister3.png)

### Second Account Microservice
![Account Microservice 2 Terminal](images/TerminalAccount2.png)
![Account Microservice 2 Browser](images/ServiceAccount2.png)

### Server Eureka
![Server Eureka 2 Browser](images/ServiceRegister2.png)



##**Brief report and kill the Account Microservice with port 2222**
![Server Eureka Kill Terminal](images/TerminalRegisterKill.png)

When someone add or kill a Microservices the WebService Microservice on port 3333 comunicates with the Registration Service on port 1111 and configure the endpoint with the Account Microservice endpoint most recently. In this way the WebService Microservice can continue to consume data from a Account Microservice even when it changes location.
