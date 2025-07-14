<div align="center">
  <h1>🚀 GoStack Desafio 09 - Node.js Template</h1>
  <p>
    <img src="https://img.shields.io/badge/Node.js-14.x-green.svg" alt="Node.js" />
    <img src="https://img.shields.io/badge/TypeScript-3.8.x-blue.svg" alt="TypeScript" />
    <img src="https://img.shields.io/badge/PostgreSQL-12.x-blue.svg" alt="PostgreSQL" />
    <img src="https://img.shields.io/badge/License-MIT-yellow.svg" alt="MIT License" />
  </p>
  <p>Template robusto, modular e escalável para aplicações Node.js com TypeScript, DDD e PostgreSQL.</p>
</div>

---

## 📑 Sumário
- [Sobre o Projeto](#-sobre-o-projeto)
- [Principais Tecnologias](#-principais-tecnologias)
- [Padrões e Arquitetura](#-padrões-e-arquitetura)
- [Configuração e Setup](#-configuração-e-setup)
- [Scripts Disponíveis](#-scripts-disponíveis)
- [Estrutura de Rotas](#-estrutura-de-rotas)
- [Licença](#-licença)

---

## 💡 Sobre o Projeto

Este template foi desenvolvido para acelerar o início de projetos Node.js utilizando as melhores práticas do mercado, como arquitetura DDD, injeção de dependência, testes automatizados e integração com PostgreSQL via TypeORM.

---

## 🛠️ Principais Tecnologias

<div align="center">
  <img src="https://img.shields.io/badge/Node.js-14.x-green.svg" />
  <img src="https://img.shields.io/badge/TypeScript-3.8.x-blue.svg" />
  <img src="https://img.shields.io/badge/Express-4.x-lightgrey.svg" />
  <img src="https://img.shields.io/badge/TypeORM-0.2.x-orange.svg" />
  <img src="https://img.shields.io/badge/tsyringe-inject-brightgreen.svg" />
  <img src="https://img.shields.io/badge/Jest-testing-red.svg" />
  <img src="https://img.shields.io/badge/ESLint-linting-blueviolet.svg" />
  <img src="https://img.shields.io/badge/Prettier-formatting-ff69b4.svg" />
</div>

- **Node.js**
- **TypeScript**
- **Express**
- **TypeORM**
- **PostgreSQL**
- **tsyringe** (Injeção de Dependência)
- **Jest** (Testes)
- **ESLint + Prettier** (Padronização de código)

---

## 🏗️ Padrões e Arquitetura

- 🔹 **Modularização/DDD:** Separação por domínio em `src/modules` (`customers`, `products`, `orders`).
- 🔹 **Camada Shared:** Código compartilhado, providers, containers e infraestrutura (`src/shared`).
- 🔹 **TypeORM:** Mapeamento objeto-relacional, migrations e entidades.
- 🔹 **Injeção de Dependência:** Utilização do `tsyringe` para desacoplamento.
- 🔹 **Rotas Express:** Modularizadas por domínio.

---

## ⚙️ Configuração e Setup

```bash
# 1. Clone o repositório
$ git clone <repo-url>
$ cd Nodejs-template--GoStack09

# 2. Instale as dependências
$ yarn install # ou npm install

# 3. Configure o banco de dados (PostgreSQL)
# Edite o arquivo ormconfig.json se necessário:
# {
#   "type": "postgres",
#   "host": "localhost",
#   "port": "5432",
#   "username": "postgres",
#   "password": "docker",
#   "database": "gostack_desafio09"
# }

# 4. Rode as migrations
$ yarn typeorm migration:run

# 5. Inicie o servidor em desenvolvimento
$ yarn dev:server
```

---

## 📜 Scripts Disponíveis

| Comando                | Descrição                                 |
|------------------------|-------------------------------------------|
| `yarn dev:server`      | Inicia o servidor em modo desenvolvimento |
| `yarn build`           | Compila o projeto para a pasta `dist`     |
| `yarn test`            | Executa os testes automatizados           |
| `yarn typeorm`         | Executa comandos do TypeORM (migrations)  |

---

## 🌐 Estrutura de Rotas

| Rota                | Método | Descrição                |
|---------------------|--------|--------------------------|
| `/customers`        | POST   | Cria um novo cliente     |
| `/products`         | POST   | Cria um novo produto     |
| `/orders`           | POST   | Cria um novo pedido      |
| `/orders/:id`       | GET    | Busca detalhes do pedido |

---

## 📝 Licença

Este projeto está sob a licença MIT.

## 👤 Autor
by **Rodolfo M. F. Abreu**

<div align="center">
  <strong>Feito com 💙 por GoStack & comunidade!</strong>
</div>
