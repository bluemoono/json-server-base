# json-server-base

Esse é o repositório com a base de JSON-Server + JSON-Server-Auth já configurada, feita para ser usada no desenvolvimento das API's nos Projetos Front-end.

## Endpoints

Assim como a documentação do JSON-Server-Auth traz (https://www.npmjs.com/package/json-server-auth), existem 3 endpoints que podem ser utilizados para cadastro e 2 endpoints que podem ser usados para login.

### Cadastro

POST /register <br/>
POST /signup <br/>
POST /users

Qualquer um desses 3 endpoints irá cadastrar o usuário na lista de "Users", sendo que os campos obrigatórios são os de email e password.
Você pode ficar a vontade para adicionar qualquer outra propriedade no corpo do cadastro dos usuários.


### Login

POST /login <br/>
POST /signin

Qualquer um desses 2 endpoints pode ser usado para realizar login com um dos usuários cadastrados na lista de "Users"

### Candies

POST /candies

Recebe dados de algum doce que você goste com a lisão de algum restaurante, com nome, ingredientes, peso e o userId.

NECESSÁRIO A AUTENTICAÇÃO POR TOKEN.

### Opinions

POST /opinions

Simula um comentário sobre o prato cadastrado, assim como em aplicativos de entrega, nele compõem com a descrição, nota, userId e candiesId (id do doce que você está comentando).

NECESSÁRIO A AUTENTICAÇÃO POR TOKEN.