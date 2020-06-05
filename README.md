# Backend do web-app Ecoleta

> RESTful API da aplicação web Ecoleta, que tem como objetivo registrar pontos de coleta de materiais recicláveis, desenvolvido na Next Level Week.
Frontend disponível nesse [repositório.](https://github.com/eduardorcury/nlw-frontend) Agradecimentos à equipe da Rocketseat pelo conteúdo excelente.

## Ferramentas

- [Node.js](https://nodejs.org/en/).
- [Typescript](https://github.com/Microsoft/TypeScript).
- Definição de rotas de acordo com o protocolo HTTP com [Express](https://github.com/expressjs/express).
- Banco de dados com [SQLite](https://www.sqlite.org/index.html).
- Ferramenta auxiliar [knex](https://github.com/knex/knex) para criação de SQL queries.

## Funcionalidades da API

### GET

Método HTTP **GET** para retorno dos items armazenados no banco de dados em formato JSON:
```
http://localhost:3333/items
```
Método HTTP **GET** para retorno dos pontos de coleta:
```
http://localhost:3333/points
```
Retorno de ponto de coleta por id:
```
http://localhost:3333/points/{id}
```
Retorno de ponto filtrados por query:
```
http://localhost:3333/points?city=Dourados&uf=MS&items=6 (EXEMPLO)
```

### POST

Método HTTP **POST** para criação de novos pontos de coleta e armazenamento no SQLite:
```
http://localhost:3333/points (POST)
```

## Como testar

Faça o download ou clonagem do repositório no seu computador.
Navegue até a pasta do projeto, abra o terminal e instale a pasta de dependências com o comando:
```
npm install
```
Em seguida, inicie o servidor com o comando:
```
npm run dev
```
É necessário ter o [Node.js](https://nodejs.org/en/) no seu computador.
Agora, você pode acessar as requisições GET no seu navegador a partir da porta *localhost:3333*.
Para testar a requisição POST, use o [Postman](https://www.postman.com/) ou [Insomnia](https://insomnia.rest/).

#### Para obter a interface do usuário, siga as instruções no [repositório do Frontend](https://github.com/eduardorcury/nlw-frontend).



