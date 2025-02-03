[![Build Status](https://app.travis-ci.com/marcelosenna1/sn-srv-ponto-inteligente.svg?token=kuokqpoxuyXRRzFqF9pc&branch=main)](https://app.travis-ci.com/marcelosenna1/sn-srv-ponto-inteligente)

# Ponto Inteligente API


## Descrição
Esta é uma API para gerenciamento de ponto eletrônico, desenvolvida em Java com Spring Boot. Ela permite o registro de entrada e saída de funcionários, controle de jornadas de trabalho e monitoramento de horas trabalhadas.

## Tecnologias Utilizadas
- **Java 17**
- **Spring Boot 3**
- **Spring Data JPA**
- **Spring Security**
- **PostgreSQL** (ou outro banco relacional de sua escolha)
- **Swagger/OpenAPI** para documentação
- **Lombok** para redução de boilerplate


## Instalação e Configuração

### Requisitos
- **JDK 17+**
- **Maven**
- **Banco de dados PostgreSQL (ou outro compatível)**

### Passos
1. Clone o repositório:
   ```sh
   git clone https://github.com/marcelosenna1/sn-srv-ponto-inteligente.git
   ```

2. Configure o banco de dados no `application.properties` ou `application.yml`:
   ```properties
   spring.datasource.url=jdbc:postgresql://localhost:5432/ponto_db
   spring.datasource.username=seu_usuario
   spring.datasource.password=sua_senha
   spring.jpa.hibernate.ddl-auto=update
   ```

## Autenticação e Segurança
A API utiliza autenticação JWT para garantir segurança. Para acessar endpoints protegidos:
1. Realize login fornecendo credenciais válidas.
2. Utilize o token retornado no cabeçalho `Authorization` para chamadas futuras:
   ```sh
   Authorization: Bearer <seu_token>
   ```

![Segurança](https://via.placeholder.com/800x400.png?text=Autentica%C3%A7%C3%A3o+e+Seguran%C3%A7a)

## Contribuição
Sinta-se à vontade para contribuir abrindo issues e pull requests.

## Licença
Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

