# Microservices with Spring Boot - Store :white_check_mark:

Microservices with Spring and best of all with _`MIT license`_:heart_eyes:, so that we can use these projects as a study or as a basis for new projects, even sharing new ideas:bulb:. Feel free to contribute to these projects right here.:hearts:

## Index :pushpin:
- [About the project](#about)
- [How to run](#run)
- [Projects and repositories](#prjrepo)
- [License](#license)

## About the project <a name="about"></a> :link:

O projeto foi desenvolvido utilizando Spring Boot, portanto foi adotado uma arquitetura baseada em micro serviços utilizando todo o poder do Spring Cloud e suas tecnologias. Quando estamos trabalhando com Spring temos diversas vantagens por ganharmos tecnologias e soluções já prontas para serem implementadas, portanto fizemos o uso de algumas delas.  

Nós quebramos o domínio da solução em 3 projetos (loja, fornecedor, transportador), sendo assim em nossas APIs nós utilizamos algumas tecnologias e soluções para construir uma arquitetura sólida, segura, rastreável e escalável. Segue abaixo. :arrow_down:

#### Netflix Eureka

- Usamos o Netflix Eureka como uma solução de Service Discovery, ela é bem simples e fácil de implementar.

#### Config Server

- As configurações yaml dos projetos foram todas exportadas e configuradas através da tecnologia dp Spring Cloud com o Config Server.

#### Spring Feign

- Foi utilizado Spring Feign para realizar chamadas entre micro serviços através de chamadas bem simples para seus clientes, é um projeto que foi inspirado em Retrofit, JAXRS-2.0 e WebSocket. Com ele nós também conseguimos utilizar o Client Side Load Balancer pois o Feign é integrado com o Ribbon, que por sua vez também é integrado com o Eureka.

#### Netflix Eureka

- Spring Cloud Sleuth was used to assist us with Distributed Tracing, responsible for implementing a distributed tracking solution, which helps us track requests between microservices through a correlation ID, so that we can track the entire flow of a request that goes through several microservices. To observe the logs we use Papertrail.


.........
Usamos o _`Netflix Hystrix`_ que implementa o padrão Circuit Breaker, que de forma bem rápida é um _`failover`_ para chamadas entre micro serviços, ou seja, caso um micro serviço estiver fora do ar um método de _`fallback`_ é chamado e aquela enxurrada de falhas é evitada.

#### Spring Cloud with Spring Boot

Building distributed systems doesn't need to be complex and error-prone. Spring Cloud offers a simple and accessible programming model to the most common distributed system patterns, helping developers build resilient, reliable, and coordinated applications. Spring Cloud is built on top of Spring Boot, making it easy for developers to get started and become productive quickly.

![Spring Cloud](img/spring-cloud.png)

## How to run <a name="run"></a> :wrench:

This project was built from a use of .....This project was built from a use of .....This project was built from a use of .....This project was built from a use of .....This project was built from a use of .....This project was built from a use of .....This project was built from a use of .....This project was built from a use of .....This project was built from a use of .....This project was built from a use of .....This project was built from a use of .....This project was built from a use of .....This project was built from a use of .....This project was built from a use of .....This project was built from a use of .....

## Projects and repositories <a name="prjrepo"></a> :file_folder:

#### Applications :computer:

- [spring-microservice-loja](https://github.com/mupezzuol/spring-microservice-loja) - Microservice related to the application of the store. _Tags: `loja`_
- [spring-microservice-fornecedor](https://github.com/mupezzuol/spring-microservice-fornecedor) - Microservice related to supplier application. _Tags: `fornecedor`_
- [spring-microservice-transportador](https://github.com/mupezzuol/spring-microservice-transportador) - Microservice related to the application of the carrier. _Tags: `transportador`_

#### Spring Cloud and Config Server :notebook_with_decorative_cover:

- [spring-microservice-config-server](https://github.com/mupezzuol/spring-microservice-config-server) - Microservice for spring cloud configuration. _Tags: `configuration`_
- [spring-microservice-config-server-repo](https://github.com/mupezzuol/spring-microservice-config-server-repo) - Microservice related to the config server repository. _Tags: `yaml`_

#### Spring Security - OAuth2 :closed_lock_with_key:

- [spring-microservice-auth](https://github.com/mupezzuol/spring-microservice-auth) - Microservice related to the application of authentication and authorization between microservices with OAuth2. _Tags: `OAuth2`, `Security`_

#### Service Registration and Discovery :mag_right:

- [spring-microservice-eureka-server](https://github.com/mupezzuol/spring-microservice-eureka-server) - Microservice related to Netflix Eureka server application. _Tags: `Eureka`_

#### API Gateway :traffic_light:

- [spring-microservice-zuul](https://github.com/mupezzuol/spring-microservice-zuul) - Microservice related to Netflix Zuul server application. _Tags: `proxy`_

#### Monitoring :chart_with_upwards_trend:

- [spring-microservice-boot-admin](https://github.com/mupezzuol/spring-microservice-boot-admin) - Microservice related to microservice monitoring with Spring Boot Admin. _Tags: `actuator`, `swagger`_

## License <a name="license"></a> :clipboard:

Feel free to contribute, we continue with an _`MIT license`_. :heart_eyes:[here](https://github.com/mupezzuol/spring-microservice-loja/blob/master/LICENSE)