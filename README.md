# Microserviço de Envio de E-mails com RabbitMQ

Microserviço responsável pelo envio de e-mails síncronos e assíncronos utilizando fila RabbitMQ (CloudAMQP).  
Parte de uma arquitetura de microsserviços com comunicação entre ms-user e ms-email.

[![Java 17+](https://img.shields.io/badge/Java-17%2B-orange?logo=java)](https://openjdk.java.net/)
[![Spring Boot 3.5](https://img.shields.io/badge/Spring_Boot-3.5-brightgreen?logo=springboot)](https://spring.io/projects/spring-boot)
[![RabbitMQ](https://img.shields.io/badge/RabbitMQ-3.12-blue?logo=rabbitmq)](https://www.rabbitmq.com/)
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-42.7-blue?logo=postgresql)](https://www.postgresql.org/)

## Funcionalidades
- Envio de e-mail direto (síncrono)
- Envio via fila RabbitMQ (assíncrono + Consumer)
- Histórico completo com status: `SENT`, `ERROR`
- Integração com Gmail SMTP / qualquer provedor
- Persistência com PostgreSQL

## Tecnologias
- Spring Boot 3.5.7
- Spring Data JPA + Hibernate
- Spring AMQP (RabbitMQ)
- Spring Mail
- Lombok
- Maven

## Como executar
```bash
./mvnw spring-boot:run
