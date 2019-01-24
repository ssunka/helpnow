# Eureka
Eureka act as a service registery/discovery for the spring boot microservices. Applications can retrieves a list of all connected peers of a service registry and makes all further requests to any other services through Eureka.

# What do you need to register your app to Eureka
You should have a Eureka client added to your app, more details here https://cloud.spring.io/spring-cloud-netflix/multi/multi__service_discovery_eureka_clients.html
In the kubernetes cluster, you use this url to register with Eureka `eureka.eureka.dev.svc.cluster.local:8761` . The same is exposed to outside world as http://hnopen-poc-app4:30061/ 
(format http://kubernetes-master:node-port/)
