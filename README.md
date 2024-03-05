# Clean Architecture com Java

Meu intuito com esse repositório é sugerir um padrão para a estruturação de um projeto usando uma arquitetura limpa. Claro que, como é apenas uma sugestão, você pode adaptá-lo para atender às necessidades do seu projeto. O importante é seguir a ideia de estruturação para que possamos tornar nossos projetos mais organizados e de fácil manutenção

Espero que isso ajude! 😊

```
seu-projeto/
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   ├── com.seunome.seuprojeto/
│   │   │   │   ├── application/
│   │   │   │   │   ├── dto/ (Data Transfer Objects)
│   │   │   │   │   ├── usecase/ (Implementação das interfaces de Use Cases)
│   │   │   │   ├── domain/
│   │   │   │   │   ├── usecase/ (Interfaces de Use Cases)
│   │   │   │   │   ├── entities/ (Entidades)
│   │   │   │   │   ├── repository/ (Interfaces de Repositório)
│   │   │   │   │   ├── service/ (Interfaces de Serviços do Domínio)
│   │   │   │   │   ├── kafka/ (Interfaces de Serviços Kafka)
│   │   │   │   │   ├── grpc/ (Interfaces de Serviços gRPC)
│   │   │   │   ├── infrastructure/
│   │   │   │   │   ├── repository/ (Implementações de Repositório)
│   │   │   │   │   ├── service/ (Implementações de Serviços do Domínio)
│   │   │   │   │   ├── web/ (Controladores, DTOs de Request/Response)
│   ├── test/
│   │   ├── java/
│   │   │   ├── com.seunome.seuprojeto/
│   │   │   │   ├── application/
│   │   │   │   │   ├── usecase/ (Testes dos Casos de Uso)
│   │   │   │   ├── domain/
│   │   │   │   │   ├── model/ (Testes das Entidades e Objetos de Valor)
│   │   │   │   ├── infrastructure/
│   │   │   │   │   ├── repository/ (Testes dos Repositórios)
│   │   │   │   │   ├── service/ (Testes dos Serviços do Domínio)
│   │   │   │   │   ├── web/ (Testes dos Controladores)
│   │   │   │   │   ├── kafka/ (Interfaces de Serviços Kafka)
│   │   │   │   │   ├── grpc/ (Interfaces de Serviços gRPC)
├──
```
Nesta estrutura:

- application: contém as implementações dos casos de uso da aplicação.
- domain:  contém as entidades, objetos de valor, interfaces de repositório e interfaces de serviços do domínio.
- infrastructure: contém as implementações de repositório, implementações de serviços do domínio e controladores.
