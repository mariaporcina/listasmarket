# ListaSmarket: Lista de Compras Inteligente

**Autor:** Maria Porcina Nogueira de Almeida

## Sobre o Projeto

Aplicativo para gestão de listas de compras.

Projeto acadêmico dedicado à disciplina de Tópicos Especiais do curso de TSI da UTFPR-GP.

## Deploy

https://lista-smarket.onrender.com/

## Instruções de Execução

**Configura arquivo `.env`**

1. Duplicar arquivo `.env.example`
2. Renomear cópia para `.env`
3. Ajustar a variável `DATABASE_URL` de acordo com o seu banco de dados

**Instalar dependencias**

```
npm i
```

**Popular Banco de Dados com Produtos e Categorias**

```
npm run seed
```

**Rodar aplicação**

```
npm run start:dev
```

A aplicação estará disponível em [`http://localhost:3000/`](http://localhost:3000/)

**(Opcional) Rodar Prisma Studio**

```
npm run prisma:studio
```

**(Opcional) Gerar build do projeto**

```
npm run build
```

## Banco de Dados

Diagrama de Entidade-Relacionamento (ERD).

**DBDiagram:** [https://dbdiagram.io/d/ListaMarket-Diagram-67eb24be4f7afba184de1a80](https://dbdiagram.io/d/ListaMarket-Diagram-67eb24be4f7afba184de1a80)

## Documentação

**Swagger:** [https://lista-smarket.onrender.com/api/v1](https://lista-smarket.onrender.com/api/v1)

## Checklist de Requisitos

### RA1 - Projetar e desenvolver uma API funcional utilizando o framework NestJS.

 - [x] ID1: O aluno configurou corretamente o ambiente de desenvolvimento e criou a API utilizando NestJS, com rotas e controladores que seguem a arquitetura modular.
 - [x] ID2: O aluno aplicou boas práticas de organização da lógica de negócios, garantindo que os services contenham a lógica de negócio e sejam chamados pelos controladores, separando responsabilidades corretamente.
 - [x] ID3: O aluno utilizou providers e configurou adequadamente a injeção de dependência no NestJS, garantindo uma arquitetura modular e escalável.
 - [x] ID4: O aluno demonstrou a habilidade de criar e manipular rotas HTTP, manipulando parâmetros de rota, query e body, lidando corretamente com requisições e respostas.
 - [x] ID5: O aluno aplicou boas práticas de tratamento de erros, utilizando filtros globais e personalizando as mensagens de erro para garantir respostas claras e consistentes.
 - [x] ID6: O aluno criou classes DTO (Data Transfer Objects) para garantir a validação e consistência dos dados em diferentes endpoints, utilizando pipes para validar entradas de dados.
 - [ ] ID7: O aluno aplicou corretamente pipes de validação no NestJS, verificando entradas inválidas e assegurando a integridade dos dados transmitidos

### RA2 - Implementar persistência de dados com um banco de dados relacional utilizando Prisma ou TypeORM.

 - [x] ID8: O aluno modelou corretamente os dados da aplicação, definindo entidades, suas relações e campos necessários, refletidos em um Diagrama de Entidade-Relacionamento (ERD).
 - [x] ID9: O aluno configurou e conectou a API a um banco de dados relacional (PostgreSQL, MySQL, etc.) utilizando Prisma ou TypeORM.
 - [x] ID10: O aluno criou e aplicou migrações de banco de dados para garantir a consistência dos dados entre desenvolvimento e produção.
 - [x] ID11: O aluno implementou corretamente as operações CRUD (Create, Read, Update, Delete) para pelo menos uma entidade no projeto, utilizando NestJS.

### RA3 - Realizar testes automatizados para garantir a qualidade da API.

 - [ ] ID12: O aluno implementou testes automatizados (unitários ou de integração) utilizando Jest, validando funcionalidades críticas da API.
 - [ ] ID13: O aluno garantiu a cobertura de testes para, pelo menos, as principais rotas e serviços da API, incluindo operações CRUD.
 
### RA4 - Gerar a documentação da API e realizar o deploy em um ambiente de produção.
 
 - [x] ID14: O aluno integrou corretamente o Swagger à API, gerando a documentação completa e interativa dos endpoints, parâmetros e respostas da API, com exemplos de requisições e respostas.
 - [x] ID15: O aluno realizou o deploy da API em uma plataforma de hospedagem na nuvem (ex.: Render.com, Heroku, Vercel, etc.), garantindo que a API estivesse acessível publicamente.
 - [x] ID16: O aluno garantiu que a API funcionasse corretamente no ambiente de produção, incluindo a documentação Swagger e o banco de dados.
 - [x] ID17: O aluno realizou a configuração correta de variáveis de ambiente usando o ConfigModule do NestJS.
 - [x] ID18: O aluno implementou corretamente o versionamento de APIs REST no NestJS, assegurando que diferentes versões da API pudessem coexistir.
 
### RA5 - Implementar autenticação, autorização e segurança em APIs utilizando JWT, Guards, Middleware e Interceptadores.
 
 - [x] ID19: O aluno configurou a autenticação na API utilizando JWT (JSON Web Tokens).
 - [x] ID20: O aluno implementou controle de acesso baseado em roles e níveis de permissão, utilizando Guards para verificar permissões em rotas específicas.
 - [x] ID21: O aluno configurou e utilizou middleware para manipular requisições antes que elas chegassem aos controladores, realizando tarefas como autenticação, logging ou tratamento de CORS.
 - [x] ID22: O aluno implementou interceptadores para realizar logging ou modificar as respostas antes de enviá-las ao cliente.
