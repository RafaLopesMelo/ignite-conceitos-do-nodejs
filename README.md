<p style="text-algn:center;">
  <img src="https://user-images.githubusercontent.com/60680170/110703768-ee88f380-81d2-11eb-94db-59234eeb7bf8.png"/>
</p>

# 🔥 - [Ignite] - Conceitos do NodeJS

## 📕 Introdução

Projeto feito no primeiro desafio da trilha de NodeJS do ![bootcamp Ignite da Rocketseat](https://passport.rocketseat.com.br/ig-nodejs-01/rafael-melo-05377). O objetivo deste desafio é fixar os conhecimentos básicos de NodeJS/Express aprendidos no primeiro e segundo módulos da trilha.

Nele construimos uma simples API capaz de criar usuários e tarefas relacionadas a esses usuários. Todos os dados são persistidos em memória e, portanto, são perdidos cada vez que o servidor é reiniciado.

## 💻 Tecnologias usadas

- NodeJS
  - Express
  
## 🎮 Como executar

#### Este projeto apenas deve ser executado em ambiente de desenvolvimento

Para executá-lo, basta instalar todas as dependências com yarn ou npm:

```bash
$ yarn
# ou
$ npm install
```

E então iniciar o servidor com o seguintes comando:

```bash
$ yarn dev
# ou
$ npm run dev
```

Para executar os testes, basta executar o seguinte comando:

```bash
$ yarn test
# ou
$ npm run test
```

## 📬 Endpoints

- POST /users
  - Cria usuário 
  - body
    - name - Nome do usuário
    - username - Apelido do usuário
    
- GET /todos
  - Retorna as tarefas de um determinado usuário
  - headers
    - username - Apelido do usuário
    
- POST /todos
  - Cria um tarefa para determinado usuário
  - headers
    - username - Apelido do usuário
  - body
    - title - Título da tarefa
    - deadline - Data limite para a tarefa
  
- PUT /todos/:id
  - Edita uma tarefa de determinado usuário
  - params
   - id - ID da tarefa
  - headers
    - username - Apelido do usuário
  - body
    - title - Título da tarefa
    - deadline - Data limite para a tarefa
   
   
- PATCH - /todos/:id/done
  - Edita uma tarefa de determinado usuário, marcando-a como feita
  - params
   - id - ID da tarefa
  - headers
    - username - Apelido do usuário
  
- DELETE - /todos/:id
  - Exclui uma tarefa de determinado usuário
  - params
   - id - ID da tarefa
  - headers
    - username - Apelido do usuário
