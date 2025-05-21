# Projeto Fullstack - N2

## Visão Geral

Este projeto consiste em um aplicativo fullstack funcional, com backend em Node.js/Express e frontend em React. O foco principal foi a construção completa do backend, incluindo modelagem de dados, segurança, desempenho e integração, além da conexão com um frontend funcional.

O backend está hospedado e acessível via URL pública, consumido pelo frontend, que permite autenticação, visualização e manipulação de dados.

---

## Arquitetura e Tecnologias

### Backend

- **Node.js** e **Express** para criação da API RESTful.
- **MongoDB** (via Mongoose) para banco de dados NoSQL.
- Modelagem clara das entidades: **Produtos**, **Pedidos**, **Clientes**, **Usuários**.
- Autenticação e autorização com **JWT** e controle por roles.
- Criptografia de senhas com **bcrypt**.
- Segurança com middlewares para CORS, rate limiting, sanitização de inputs.
- Validação dos dados com **express-validator**.
- Otimizações nas queries usando `.select()` e `.lean()`.
- Paginação e filtros via query string.
- Tratamento global de erros com mensagens claras e amigáveis.
- Middlewares adicionais para logs e permissões específicas.

### Frontend

- Construído com **React** e **Vite**.
- Conexão ao backend usando **axios** para consumir APIs.
- Páginas para autenticação, listagem e manipulação de Produtos, Pedidos e Clientes.
- Sistema básico de proteção de rotas para usuários autenticados e admin.
- Interface funcional para testes (não estilizada).

### Hospedagem e Integração

- Backend hospedado no Render (ou plataforma similar).
- Frontend hospedado no Vercel (ou plataforma similar).
- Banco de dados hospedado no MongoDB Atlas.
- Comunicação segura via HTTPS com CORS e tokens JWT configurados.

---

## Funcionalidades Implementadas

- Registro e login com autenticação JWT.
- CRUD completo para Produtos, Pedidos e Clientes (criação, leitura, atualização).
- Busca, filtros e paginação nas listas via query string.
- Segurança reforçada com criptografia de senhas, sanitização e rate limiting.
- Tratamento global e detalhado de erros.
- Middleware de autorização baseado em roles.
- Frontend consumindo API, com roteamento protegido.

---

## O que falta implementar

- Finalizar testes automatizados (unitários e integração) com Jest e Supertest.
- Middleware personalizado para logs detalhados.
- Autorização fina para permissões específicas (além de roles).
- Aprimoramento da interface frontend para melhor UX/UI.
- Implementação de melhorias de performance para escalabilidade.

---

## Como rodar localmente

1. Clone o repositório:

```bash
git clone https://github.com/jvbaracho/fullstackN2.git
cd fullstackN2

    Instale dependências no backend:

cd backend
npm install

    Configure as variáveis de ambiente (.env), incluindo URI do MongoDB, segredo JWT, etc.

    Rode o backend:

npm run dev

    Em outro terminal, instale e rode o frontend:

cd ../frontend
npm install
npm run dev

    Acesse o frontend pelo endereço exibido no terminal (ex: http://localhost:3000).

Links Importantes

    Repositório: https://github.com/jvbaracho/fullstackN2

    Aplicação Online: (inserir URL pública da aplicação)

Relatório de Mudanças

    Arquitetura inicial construída com Node.js/Express e React.

    Implementação da autenticação JWT e autorização por roles.

    Modelagem e CRUD para Produtos, Pedidos e Clientes.

    Segurança reforçada com middlewares de sanitização, CORS, rate limiting.

    Otimizações de queries com projeções e uso de .lean().

    Frontend básico funcional consumindo a API.

    Tratamento global de erros implementado.

Contato

Email: jvbaracho2004@gmail.com

Obrigado por avaliar o projeto! Fico aberto a sugestões e melhorias.
