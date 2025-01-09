<h1 align="center">API COM JWT</h1>

## SOBRE

Esta é uma API que implementa autenticação baseada em JWT (JSON Web Token) utilizando o framework Laravel. A API permite o registro de usuários, login, logout, atualização de tokens e a obtenção de informações do usuário autenticado.

##  Configuração do Ambiente

- Laravel: Framework do PHP.
- JWT
- Banco de Dados:MySQL.
- Postman: Para testar as rotas.

 ## Endpoints

| Método HTTP | Endpoint       | Descrição                            | Middleware        |
|-------------|----------------|--------------------------------------|-------------------|
| POST        | /auth/register | Registra um novo usuário             | `api`             |
| POST        | /auth/login    | Realiza o login do usuário           | `api`             |
| POST        | /auth/logout   | Realiza o logout do usuário          | `api`, `auth:api` |
| POST        | /auth/refresh  | Atualiza o token JWT                 | `api`, `auth:api` |
| POST        | /auth/me       | Recupera informações do usuário      | `api`, `auth:api` |


 ## Licença

Este projeto está licenciado sob os termos da MIT License.