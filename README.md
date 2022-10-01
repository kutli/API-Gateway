#API Gateway

The API Gateway exist one layer above the eureka server and act as a load balancer for the micro-services registered 
in the discovery service


## Run in Local:
The app will start in local server in port 8082.
You must run the eureka server(discovery service) so the api gateway can be registered.

### Call a microsevice registered in eureka by the api gateway

```localhost:8082/tacos-service/PATH```





## ENV VARS that must be configured in server:
EUREKA_HOSTNAME: Host name of the api gateway<br />
EUREKA_URL: url of eureka server(discovery service) with user and password

### Example of env vars in heroku
```
EUREKA_HOSTNAME=my_api_gateway.herokuapp.com
EUREKA_URL=https://user:password@eureka-server.herokuapp.com/
```
