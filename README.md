# bank-app-ws-cloud-eureka
![ban-app schema](schema.PNG)

## Les modules : 

- discovery-service : Eureka
- gateway : Spring-cloud & gateway
- customer-service & account-service : Spring Boot
- config-service : spring-cloud-config & actuator

## Les technologies utilisées : 

  - Spring Boot
  - JPA / Hibernate / Spring Data
  - H2 database
  - Lombok
  - Spring Doc (swagger)
  - Spring Cloud
  - Actuator : pour voir l'état du ws
  - Eureka : pour registrer les ws démarrer et pour faciliter le dispatching du gateway vers les ws
  - Spring cloud config server : pour centraliser les configs des ws dans un seul projet (config-service) et globaler les configs partagés entre plusieurs ws.
  - Resilience 4j : pour que si l'un des ws DOWN n'impact pas les autres ws et on lui fournir une réponse par défaut en cas de problème.
  - OpenFeign est une bibliothèque Java qui simplifie le développement de clients HTTP en utilisant une interface déclarative. Elle fait partie de la suite Spring Cloud et est souvent utilisée dans les applications basées sur microservices.
