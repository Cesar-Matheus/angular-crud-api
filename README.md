# Atividade Didática: Integração com APIs

Este projeto é destinado aos alunos da unidade curricular **Interação com APIs**. O objetivo desta atividade é colocar em prática a integração de um projeto Front-End (Angular) com um Back-End (Node.js/Express) utilizando o `HttpClient`.

O Back-End já está totalmente desenvolvido e funcional. O Front-End já está criado com as telas e formulários prontos, mas faltam as chamadas HTTP. **A sua tarefa é implementar a comunicação entre os dois.**

## Estrutura do Projeto

O repositório está dividido em duas partes principais:

- `frontend/`: O projeto Angular (UI).
- `backend/`: A API Node.js/Express.

## Pré-requisitos

Certifique-se de ter instalado em sua máquina:
- [Node.js](https://nodejs.org/) (versão LTS recomendada)
- NPM (já vem com o Node.js)

## Como executar o projeto

Para que o sistema funcione corretamente, você precisará executar o Back-End e o Front-End simultaneamente em dois terminais separados.

### 1. Back-End

Abra o primeiro terminal, navegue até a pasta do back-end, instale as dependências e inicie o servidor:

```bash
cd backend
npm install
npm run dev
```
*(O Back-End ficará rodando no endereço: `http://localhost:3000/api`)*

### 2. Front-End

Abra um segundo terminal, navegue até a pasta do front-end, instale as dependências e inicie a aplicação Angular:

```bash
cd frontend
npm install
npm start
```
*(O Front-End ficará acessível no endereço: `http://localhost:4200`)*

**Importante**: Mantenha os dois terminais abertos enquanto estiver desenvolvendo.

## Endpoints Disponíveis no Back-End

A API trabalha com os seguintes endpoints no endereço base `http://localhost:3000`:

| Método | Endpoint            | Descrição              |
| ------ | ------------------- | ---------------------- |
| GET    | `/api/products`     | Listar todos produtos  |
| GET    | `/api/products/:id` | Consultar um produto   |
| POST   | `/api/products`     | Cadastrar um produto   |
| PUT    | `/api/products/:id` | Atualizar um produto   |
| DELETE | `/api/products/:id` | Excluir um produto     |

*Dica: Você pode testar essas rotas no **Postman** (ou Insomnia) antes de implementá-las no Angular para ver como os dados são retornados ou recebidos.*

## Parte que os alunos deverão implementar

Sua tarefa consiste em implementar os métodos vazios do serviço `ProdutoService` localizado em:
`frontend/src/app/produtos/produto.service.ts`

Você deverá utilizar o `HttpClient` do Angular (já injetado na classe) para realizar as chamadas aos endpoints da API listados acima, substituindo os retornos provisórios.

Bom trabalho!
