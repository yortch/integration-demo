# spring-integration-demo
Even in 2019, we often still need to develop SOAP based web services due to legacy applications. 
It was hard to find code samples that use Spring Integration with Java DSL using Spring Boot to expose/consume SOAP based web services.
This repo will show some code examples using all of the above.

1. [initial](https://github.com/yortch/spring-integration-demo/tree/initial) branch shows an initial implementation of a web service exposed using spring-ws, Spring Boot and Java DSL. This was loosely based on the ["Producing a SOAP web service" getting started guide](https://spring.io/guides/gs/producing-web-service/).
1. [inboundgateway](https://github.com/yortch/spring-integration-demo/tree/inboundgateway) branch takes the initial branch and converts it to using Spring Integration classes (i.e. `MarshallingWebServiceInboundGateway` and `MessageChannel`). Credit to [tomask79's spring boot web service integration repo](https://bitbucket.org/tomask79/spring-boot-webservice-integration/src/master/) which was one of few sample codes I found to expose a SOAP services using Spring Integration with Java DSL. In particular this [commit](https://github.com/yortch/spring-integration-demo/commit/c95b4cbf6108e413072dda57ddf2d7528bb39ff5) will show you how easy it is to go from Spring-WS to a Spring Integration implementation.
