# Log-Gateway

This acts as a gateway to compare the two different logs.
It is utilizing 
1) Spring Netflix Zuul ---> Utilizing to customize the web request before routing to the actual backend services to fetch the logs
2) Spring config ----> Separate config for the different stages of an application in order to configure different databases
3) Spring Eureka Discovery ----> How to find and connect with service to fetch the log hosted on different server without hard coding the server details
4) Spring REST API -----> API calls to add and retrieve the api and store the logs.
5) Spring Eureka ----> Going over server load balancing with the Eureka 
