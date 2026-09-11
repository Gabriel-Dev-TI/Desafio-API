# Desafio API

API RESTful em Laravel com autenticação via token (Sanctum) para consumo no Flutter.

## Stack

- **Backend:** Laravel 
- **Auth:** Laravel Sanctum (token Bearer)
- **Banco:** MySQL
- **Hospedagem:** Wasmer Edge
- **Frontend:** Flutter (consumidor)

## Endpoints

| Método | Rota | Auth | Descrição |
|--------|------|------|-----------|
| POST | `/api/register` | Não | Cria conta e retorna token |
| POST | `/api/login` | Não | Autentica e retorna token |
| GET | `/api/user` | Sim | Retorna dados do usuário logado |
| POST | `/api/logout` | Sim | Invalida o token atual |