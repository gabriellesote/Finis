# Descrição dos Diagramas

## Diagrama de usuário

### User  <\<entity>>
- Classe de domínio
- Reflete a tabela users no banco

### UserController <\<controller>>
- Controla requisições HTTP (ex: /login, /register, etc)
- Recebe DTOs como RegisterDTO ou LoginDTO
- Chama o UserService


### UserService <\<service>>
- Implementa regras de negócio
- Pode validar dados, aplicar lógica, transformar DTO → Entity
- Chama o UserDAO

### UserDAO <\<repository>>
- Cuida da persistência de dados (normalmente via JPA/Hibernate ou SQL)
- Só acessa o banco de dados, sem lógica de negócio

### DTOs (RegisterDTO, LoginDTO, ProfileDTO)
- Usados para entrada ou saída de dados
- Não devem conter lógica
- Evitam expor a Entity diretamente

### Resumo

| Camada     | Responsabilidade Principal                           |
| ---------- | ---------------------------------------------------- |
| Controller | Receber requisições, validar entrada, chamar service |
| Service    | Aplicar regras de negócio, orquestrar                |
| DAO/Repo   | Acessar banco de dados                               |
| DTO        | Transportar dados entre camadas                      |
| Entity     | Representar o domínio/modelo                         |


