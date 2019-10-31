# Log-Gateway

A Simple REST API's to compare the log files hosted on different servers.

1) Add an apis 
2) Fetch api logs
3) Compare based on the given user entered filters

It is utilizing 
1) Spring Netflix Zuul ---> To customize the http requests before routing to the actual backend api calls.
2) Spring Config ----> Configuration for the different stages of an application (currently I have local but there could be dev,test,prod etc.) 
3) Spring Eureka Discovery ----> To find and connect with service to fetch the log hosted on different server without hard coding the actualt server details.
4) Spring REST API -----> API calls to add, retrieve api details and store the logs.
5) Spring Eureka ----> Server load balancing with the Eureka 
