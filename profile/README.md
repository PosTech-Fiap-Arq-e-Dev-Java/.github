
## Tech Challenge FIAP - Pós-graduação em Arquitetura e Desenvolvimento Java

📄 **Documentação Oficial do Desafio**  
[Repositórios desenvolvidos para o Tech Challenge da FIAP, com foco em arquitetura moderna utilizando microsserviços, Clean Architecture e abordagem API First.](https://docs.google.com/document/d/e/2PACX-1vSw_auwVeiZGyAN7WkUH30ksHZ-HE-bz1kVepJj2s0bZP-Z4Ff69cy3S0-nEj-yYYv37Y9cB4-EIR2l/pub)

🎥 **Vídeo de Apresentação**  
_[Link da apresentação em vídeo](https://youtu.be/dtWbzXhYaAU)_

---

## ⚙️ Arquitetura de Microsserviços - Gestão de Usuários, Login e Cardápio

Este projeto é composto por múltiplos microsserviços que interagem entre si para prover uma solução completa de gerenciamento de usuários (clientes e restaurantes), autenticação e gerenciamento de cardápio.

### 🔧 Pilares Arquiteturais

- Microsserviços
- Clean Architecture
- API First (OpenAPI Generator)

---

## 🧩 Microsserviços

### 🔹 [`ms-login`](https://github.com/PosTech-Fiap-Arq-e-Dev-Java/ms-login)

Responsável pela **autenticação** de usuários (cliente e restaurante), incluindo criação, atualização, exclusão de login e alteração de senha.

### 🔹 [`ms-usuario`](https://github.com/PosTech-Fiap-Arq-e-Dev-Java/ms-usuario)

Gerencia **dados de usuários**, tanto clientes quanto restaurantes. Inclui criação, edição, exclusão e consulta de dados cadastrais.

### 🔹 [`ms-cardapio`](https://github.com/PosTech-Fiap-Arq-e-Dev-Java/ms-cardapio)

Permite a **gestão de cardápios** de restaurantes: adicionar, remover e editar itens de menu e tipos de cozinha.

---

## 🐳 Docker & Integração

### [`docker`](https://github.com/PosTech-Fiap-Arq-e-Dev-Java/docker)

Contém o `docker-compose.yml` responsável por subir os bancos de dados e preparar o ambiente de execução dos microsserviços.

---

## 🧪 Testes de API

### [`collections`](https://github.com/PosTech-Fiap-Arq-e-Dev-Java/collections)

Coleções do Postman com testes para validar os endpoints dos microsserviços de forma manual e/ou automatizada.

---

## ⚙️ Tecnologias Utilizadas

| Tecnologia           | Descrição                                      |
|----------------------|-----------------------------------------------|
| Java 21              | Linguagem principal                            |
| Spring Boot          | Framework para desenvolvimento de APIs REST   |
| Spring Data JPA      | Abstração de persistência                      |
| OpenAPI Generator    | API First (geração de contratos e client SDK) |
| Lombok               | Redução de boilerplate                        |
| MapStruct            | Conversão entre DTOs e domínios               |
| JUnit + Mockito      | Testes unitários e mocks                      |
| Docker               | Conteinerização dos bancos                    |
| Git                  | Versionamento                                 |
| Postman              | Testes de API                                 |

---

## 🧪 Estratégia de Testes

- **Unitários:** JUnit 5 + Mockito
- **APIs:** Postman (com coleções versionadas no repositório [collections](https://github.com/PosTech-Fiap-Arq-e-Dev-Java/collections))

---


## 🐳 Execução com Docker Compose

### ✅ Pré-requisitos

| Requisito   | Descrição                                                                 |
|-------------|---------------------------------------------------------------------------|
| Docker      | Necessário para rodar os containers dos bancos                           |
| Java 21+    | Para executar os microsserviços                                           |
| Postman     | Para testes manuais com as collections                                    |
| Git         | Para clonar os repositórios                                               |
| DBeaver     | (Opcional) Visualização gráfica dos bancos de dados                      |

---

## 💻 Como usar

### 🐧 Linux / macOS

```bash
chmod +x setup.sh
./setup.sh
## Contrato OpenAPI

A API foi desenvolvida com abordagem **API First** utilizando OpenAPI. O contrato está disponível no repositório.

## Execução com Docker

Há um arquivo `docker-compose.yml` na pasta `docker/`, que pode ser utilizado para subir o ambiente com MySQL e o microsserviço.

### Instruções

```bash
cd docker
docker-compose up --build
```

## Repositórios Relacionados

- [ms-login](https://github.com/PosTech-Fiap-Arq-e-Dev-Java/ms-login)
- [ms-usuario](https://github.com/PosTech-Fiap-Arq-e-Dev-Java/ms-usuario)
- [ms-cardapio](https://github.com/PosTech-Fiap-Arq-e-Dev-Java/ms-cardapio)

## Autor

Raysse @2025 - Projeto FIAP Pós-Tech - Arquitetura e Desenvolvimento Java.
