# NLW 4 - Rocketseat

## Tecnologias utilizadas

##### [Node](https://nodejs.org/)
##### [Express](https://expressjs.com/)
`yarn add express`

##### [Typescript](https://www.typescriptlang.org/)
``

##### [Sqlite3](https://www.sqlite.org/index.html)
`yarn add sqlite3`

##### [TypeORM](https://typeorm.io/)
`yarn add typeorm reflect-metadata`
`yarn typeorm migration:create -n CreateUsers`
`yarn typeorm migration:run`
`yarn typeorm migration:revert`

`yarn add uuid`
`yarn add @types/uuid -D`

##### Criando nova migration
`yarn typeorm migration:create -n CreateSurveys`
`yarn typeorm migration:run`


* SQLite extension || Beekeeper Studio


## Testes automatizados
1. Testes unitários
São utilizados com TDD (Desenvolvimento Orientado a Testes).

2. Testes de integração
Testa a funcionalidade completa da aplicação.
Um teste de criação de usuário deve testar o acesso às rotas, ao controller, ao repositório, faz a criação e monta a resposta.
request -> routes -> controller -> repository
<- repository <- controller <- response

3. Testes ponta a ponta (E2E - end to end)
Mais utilizado em aplicações front-end.

##### [Jest](https://jestjs.io/pt-BR/)
`yarn add jest @types/jest -D`
`yarn jest --init`
`yarn add ts-jest -D` 

`yarn test`

Simula a inicialização de um servidor
`yarn add supertest @types/supertest -D`

## Variáveis de ambiente
"test": "set NODE_ENV=test&&jest",
"posttest": "del ./src/database/database.test.sqlite"

##### Criando nova migration
`yarn typeorm migration:create -n CreateSurveysUsers`
`yarn typeorm migration:run`