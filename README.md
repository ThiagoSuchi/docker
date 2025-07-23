# DioWallet - Mini Projeto Fullstack

Este mini projeto tem como objetivo principal aprimorar os estudos em **Docker**, integrando uma API Node.js (Express + MongoDB) e uma SPA em React, simulando uma carteira digital simples.

## Objetivo

O projeto foi desenvolvido para praticar conceitos de:
- **Containerização** de aplicações backend e frontend com Docker
- Integração entre frontend (SPA React) e backend (API Node.js)
- Utilização de banco de dados MongoDB em ambiente Docker
- Práticas de autenticação, rotas protegidas e manipulação de dados

## Estrutura

- **api/**: Backend Node.js com Express, MongoDB, autenticação JWT, validação com Joi.
- **spa/**: Frontend React com Vite, TailwindCSS, React Router, integração com API.

## Como rodar a aplicação

### Pré-requisitos

- [Docker](https://www.docker.com/) e [Docker Compose](https://docs.docker.com/compose/) instalados

### 1. Suba o MongoDB com Docker

Você pode rodar um container MongoDB com o comando:

```sh
docker run --name mongo-wallet -d -p 27017:27017 mongo