===============================
PEDIDO-SERVICE - TECH CHALLENGE
===============================

Microsserviço responsável pela criação e gerenciamento de pedidos no sistema de pedidos distribuído do Tech Challenge.

-------------------------------
📦 TECNOLOGIAS UTILIZADAS
-------------------------------
- Java 17
- Spring Boot
- Spring Web
- Spring Data JPA
- PostgreSQL
- Docker
- Maven
- Lombok

-------------------------------
📁 ESTRUTURA DO PROJETO
-------------------------------
src/
├── main/
│   ├── java/
│   │   └── br.com.techchallenge.pedido/
│   │       ├── application/    -> Controllers (API REST)
│   │       ├── core/           -> Domínio, entidades e interfaces
│   │       └── infrastructure/ -> Repositórios e configuração
│   └── resources/
│       ├── application.yml     -> Configurações do serviço
│       └── ...                 -> Outros recursos
└── test/                       -> Testes unitários e de integração

-------------------------------
⚙️ COMO EXECUTAR LOCALMENTE
-------------------------------
1. Verifique se o Docker está instalado e em execução.
2. Execute o comando:
   docker compose up --build

O serviço estará disponível em: http://localhost:8082

-------------------------------
🔁 ENDPOINTS PRINCIPAIS
-------------------------------
GET     /pedidos           - Lista todos os pedidos
POST    /pedidos           - Cria um novo pedido
GET     /pedidos/{id}      - Busca um pedido por ID
PUT     /pedidos/{id}      - Atualiza um pedido existente
DELETE  /pedidos/{id}      - Remove um pedido

-------------------------------
✅ TESTES
-------------------------------
Os testes estão em `src/test`.

Para executar:
> mvn test

Para gerar cobertura de testes:
> mvn jacoco:report

O relatório estará disponível em:
target/site/jacoco/index.html

-------------------------------
📌 OBSERVAÇÕES
-------------------------------
- Este microsserviço compõe a arquitetura distribuída do sistema de pedidos.
- Banco de dados PostgreSQL configurável via `application.yml`.
- Comunicação com outros microsserviços via REST.

-------------------------------
👩‍💻 DESENVOLVIDO POR
-------------------------------
Ludmila Moreira - Tech Challenge 2025

